## Comics Config? What is it for?
This one is very much inspired by [comic_selectors](https://github.com/oseparovic/comic_selectors) by [oseparovic](https://github.com/oseparovic/). The list there acts as a backend selector for the wonderful app named [PageFlip which is a comic reader app on Android](https://play.google.com/store/apps/details?id=com.printandpixel.pageflip2&hl=en_US).

But here we have a more generic purpose, of collecting the comic strips and an info about them (how to traverse them with CSS selectors) as a common database.

The config is in the format of the json, where each json element consists of the following keys:
```json
"title": "Adam@Home",
"author": "Rob Harrell",
"source": "gocomics.com",
"url": "https://www.gocomics.com/adamathome/1995/06/20",
"image": {
    "selector": ".item-comic-image img",
    "index": "0"
},
"first_comic": {
    "selector": ".fa-backward",
    "index": "0"
},
"last_comic": {
    "selector": ".fa-forward",
    "index": "0"
},
"previous_comic": {
    "selector": ".fa-caret-left",
    "index": "0"
},
"next_comic": {
    "selector": ".fa-caret-right",
    "index": "0"
},
"random_comic": {
    "selector": ".gc-calendar-nav__select > a.btn-outline-secondary",
    "index": "0"
}
```

**title**: A title of the comic  
**author**: An author of the comic  
**source**: Source - from where did we got this information  
**url**: The url which we can use to play with following selectors  
**image**: selectors on how to get the image  
**image.selector**: css selector on the page to fetch the image  
**image.index**: index on the above selector - where image can be found  
**first_comic**: selectors on how to get the link of the first comic  
**first_comic.selector**: css selector on the page to fetch the link of the first comic  
**first_comic.index**: index on the above selector - where link can be found  
**last_comic**: selectors on how to get the link of the last comic  
**last_comic.selector**: css selector on the page to fetch the link of the last comic  
**last_comic.index**: index on the above selector - where link can be found  
**previous_comic**: selectors on how to get the link of the previous comic  
**previous_comic.selector**: css selector on the page to fetch the link of the previous comic  
**previous_comic.index**: index on the above selector - where link can be found  
**next_comic**: selectors on how to get the link of the next comic  
**next_comic.selector**: css selector on the page to fetch the link of the next comic  
**next_comic.index**: index on the above selector - where link can be found  
**random_comic**: selectors on how to get the link of the random comic  
**random_comic.selector**: css selector on the page to fetch the link of the random comic  
**random_comic.index**: index on the above selector - where link can be found  

### If you want to contribute, how can check if you have correctly configured the CSS selectors?
The steps are same as the one mentioned on [https://github.com/oseparovic/comic_selectors](https://github.com/oseparovic/comic_selectors), till the time we add proper testing tools for automatically validating the configs.

## Issues
Feel free to [open an issue](https://github.com/codeat3/comics-config/issues/new), if you have any. Or use the same to throw a question at us.