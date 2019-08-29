This is the full email html code.
I also made the logic for the two different buttons using liquid
    {% if custom_attribute.{loyalty.has_account} == false %}
    {% capture destinationUrl %}https://www.thirdlove.com/account/register {% endcapture %}
    {% capture buttonText %}Sing up Now{% endcapture %}
    {% else %}
    {% capture destinationUrl %} https://www.thirdlove.com/account/login {% endcapture %}
    {% capture buttonText %} Sing in Now {% endcapture %}
    {% endif %}} <a href="{{destinationUrl}}"><p>{{buttonText}}</p></a>
I didn't find a way to test this on my pc after a lot of reasearching, so I decided to show one of the options on screen and drop the liquid code as a comment here and in the html.