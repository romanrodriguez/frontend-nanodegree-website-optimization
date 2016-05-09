## Website Performance Optimization portfolio project

Check out the project's page following this link: [Website Optimization](http://romanrodriguez.github.io/frontend-nanodegree-website-optimization/).

This project consists of improving an online portfolio for speed by optimizing the critical rendering path and making the page render as quickly as possible.

#### Part 1: Optimize PageSpeed Insights score for index.html

##### Results achieved: 
PageSpeed Insights on Desktop (96/100) and Mobile (97/100)

##### Optimizations performed:

* Inline CSS styling in `index.html`
* Optimized Images
* Minified JavaScript

#### Part 2: Optimize Frames per Second in pizza.html

##### Results achieved:
To optimize `views/pizza.html`, I modified `views/js/main.js` until the frames per second rate were 60 fps or higher.

##### Optimizations performed:

* Inline CSS styling in `pizza.html`
* Optimized Images
* Modified CSS `.mover` in `style.css` and `pizza.html` inline CSS to increase the site's performance with hardware accelerated CSS.
* Modifications to the `main.js` code:

1. Modified the `changePizzaSizes` function with a new variable randomPizza, and moved the `dx` and `newwidth` variables outside the for loop with it for a more efficient loop.

2. Modified the Pizza Generator function `document.addEventListener` to be more efficient by reducing the number of pizzas generated to populate the page to the minimum required. Also removed the process of resizing. 

3. Added `cachedScrollTop` outside the for loop in `updatePositions`.

#### Tools used:
* [Grunt](http://gruntjs.com/)
* [CSS Minifier](http://cssminifier.com/)
* [JS Compress](http://jscompress.com/)
* [Kraken.io](http://kraken.io/)
* [Unminify](http://unminify.com)
