## Website Performance Optimization portfolio project

This projects consists of improving an online portfolio for speed by optimizing the critical rendering path and make the page render as quickly as possible.

### Optimizations
####Part 1: Optimize PageSpeed Insights score for index.html

Results achieved: PageSpeed Insights on Desktop (96/100) and Mobile (97/100)



####Part 2: Optimize Frames per Second in pizza.html

Results achieved: PageSpeed over 60 fps (while scrolling) and under 5 ms to resize.

To optimize views/pizza.html, I modified views/js/main.js until the frames per second rate were 60 fps or higher.


Modifications to the code:

1. Modified the changePizzaSizes function with a new variable randomPizza, and moved the dx and newwidth variables outside the for loop with it for a more efficient loop.

2. Modified the Pizza Generator function document.addEventListener to be more efficient by reducing the number of pizzas generated to populate the page to the minimum required. Also removed the process of resizing. 

3. Added cachedScrollTop outside the for loop in updatePositions



Tools used:
Grunt
