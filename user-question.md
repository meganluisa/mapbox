
---

> Hi Mittens,
Thank you for reaching out! I am sorry to hear you are having issues with your site, but I looked into this and am happy to provide assistance.
Everything looks great, however, what you need to do is add `map.resize();` after line 73 (`myMap.setAttribute("style", "height:200px");`) in your `index.html` file.
This is because in order to display correctly, the map needs to be explicitly told with the [resize property](https://docs.mapbox.com/mapbox-gl-js/api/map/#map#resize) that its container changed size from what was originally defined. This has to do with the amount of space the browser calculates for each element on the page, which can be explained further on our [troubleshooting page for this issue](https://docs.mapbox.com/help/troubleshooting/blank-tiles/#your-map-is-hidden).
I hope this helps, and please let me know if you have any further questions.
Best,
Megan
