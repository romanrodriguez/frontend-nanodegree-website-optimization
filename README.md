## Website Performance Optimization portfolio project

Check out the project's page following this link: [Website Optimization](http://romanrodriguez.github.io/frontend-nanodegree-website-optimization/).

This project consists of improving an online portfolio for speed by optimizing the critical rendering path and making the page render as quickly as possible.

#### Part 1: Optimize PageSpeed Insights score for index.html

##### Results achieved: 
PageSpeed Insights on Desktop (97/100) and Mobile (95/100). User Experience 
(100/100).

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
* Modified CSS `.mover` in `views/style.css` and `pizza.html` inline CSS to increase the site's performance with hardware accelerated CSS and added vendor prefixes for better browser compatibility.
* Modifications to the `main.js` code:

1. Modified the `changeSliderLabel`  and the `determineDx` functions as the document.getElementById() Web API call is faster than document.querySelector() and the `randomPizza` and `updatePositions` functions were modified with document.getElementsByClassName() instead of querySelectorAll() as it is also faster that way.

2. Modified the `changePizzaSizes` function with a new variable randomPizza, and moved the `dx` and `newwidth` variables outside the for loop with it for a more efficient loop.

3. Declared the `pizzasDiv` variable outside the loop, so the function only makes one DOM call. 

4. Declared the phase variable in the `updatePositions` function outside the loop to prevent it from being created every time the loop is executed.

5. Modified the Pizza Generator function `document.addEventListener` to be more efficient by reducing the number of pizzas generated to populate the page to the minimum required. Moved the elem variable outside the for loop to prevent it from being created every time the loop is executed. Added the movingPizzas1tag variable outside the for loop in the `addEventListener` function.
