# Website-Optimization-Project-Udacity-
FrontEnd Developer Nanodegree Project


# Get this Page running:

1. Open index.html in the browser. 

2. To open the Pizzaria webpage open the file views, then open pizza.html in the browser, 
or choose it from fromthe index.html webpage displaying Cameron's portfolio.

## Changes made to achieve over 90 score on google Developer's PageInsights website: 

1. The css files (print.css and style.css) were inlined in the index.html

  file each contained in a style tag instead of being linked to a seperate css file 

  to avoid render blocking.

2. The googlefonts css is also inlined for the same reason.

3. The css in all the style tags are minified by removing all spaces inbetween the content.

4. The javascript script tags are async.


## Changes made in main.js and pizza.html to render the Pizzaria webpage in 60 FPS:

1. CSS is inlined in the pizza.html and the script is async-ed as in index.html.

2. In sizeSwitcher() function:
  
  The slider value are modified to percent values of screen width.

3. Function changePizaSizes():

  Used getElementsByClassName instead of querySelectorAll.

  Variables dx and newwidth are defined outside the for loop.

4. Function updatePositions():

  Through console.log test lines for the variables that were previously defined

  inside the for loop, the var phase variable showed that it doesn't change upon scrolling, so it was moved 

  outside the for loop in the updatePositions() function.
