# NordPool Curent Price

Fetches electricity prices from NordPool exchange and displays the current price for the Baltic countries in their correct time zone.

[Deployed here](https://nordpoolprice.codeborne.com/)

Useful if your electricity bill is tied to the exchange spot price, so you can decide when to charge your electric car, etc.

Source of data:
https://www.nordpoolgroup.com/Market-data1/Dayahead/Area-Prices/EE/Hourly/

## Development

Server-side runs using node (to fetch and transform the data).

Client side does not require any build steps:
* ES modules used directly in the browser
* Web Components (using lightweight [lit-element](https://www.skypack.dev/view/lit-element))
* Dependencies loaded using [Skypack](https://skypack.dev)

Use `npm start` to run locally.

## Additional information

Web components are also great for SEO (reminds me of Interflora): you can keep content in the html for crawlers to see, but use web components to make the page dynamic and reactive.

More details about Web Components:
https://developer.mozilla.org/en-US/docs/Web/Web_Components

I used lit-element to make writing web components easier:
https://lit-element.polymer-project.org/

And it is served by Skypack: https://www.skypack.dev/
Which is made by the same people as Snowpack.

And finally, highly recommended read on micro frontends using web components:
https://micro-frontends.org/
