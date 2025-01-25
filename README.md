# CSS `calc()` Inconsistency

This repository demonstrates an uncommon issue with the CSS `calc()` function when combining percentages and pixel values. The problem lies in how browsers interpret and calculate subtractions involving percentages and fixed units.

## The Problem

The provided `bug.css` demonstrates the issue. The goal was to create a sidebar (20% of viewport width minus 10px) and a main content area (the remaining 80% plus 10px).  However, the result might differ from expectations due to browser-specific interpretations of the `calc()` function.

## The Solution

The solution in `bugSolution.css` offers a workaround using a more robust approach, avoiding the direct subtraction of pixels from percentages in `calc()`. This approach prioritizes a more predictable layout across different browsers and viewport sizes. 