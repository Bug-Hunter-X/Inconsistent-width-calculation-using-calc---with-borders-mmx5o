# Inconsistent width calculation using calc() with borders

This repository demonstrates an uncommon CSS bug related to the `calc()` function and borders. Some browsers may miscalculate the width of an element when using `calc()` to set the width and also applying a border.

## Bug Description
The `calc()` function is used to dynamically calculate the width of a div element.  When a border is added, some browsers incorrectly calculate the width, leading to unexpected rendering.

## Reproduction
1. Clone this repository.
2. Open `bug.html` in different browsers (e.g., Chrome, Firefox, Edge).
3. Observe the differences in the rendering of the div element.

## Solution
The solution involves explicitly accounting for the border width in the `calc()` calculation.