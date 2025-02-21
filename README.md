# CSS Calc() Unexpected Results
This example demonstrates an uncommon issue when using the CSS `calc()` function with percentages and fixed units (like pixels) in nested or relatively sized elements.

The problem arises because `calc()` performs calculations relative to the containing element's size, not the entire viewport or parent element if it's not 100% wide.

**bug.css** shows the incorrect implementation and **bugSolution.css** offers potential solutions.

## Solutions
Consider using viewport units (vw, vh) for more predictable calculations based on the entire screen size or adjust the calculation based on the containing elements actual size using Javascript.