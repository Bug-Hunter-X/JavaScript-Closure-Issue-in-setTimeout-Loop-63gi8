# JavaScript Closure Issue in setTimeout Loop

This repository demonstrates a common issue with closures in JavaScript when using `setTimeout` within a loop.  The problem arises because the closures created by `setTimeout` do not capture the value of `i` at the time of their creation, but rather capture a reference to the variable itself.  This results in all the closures logging the final value of `i` (which is 10) instead of the expected values from 0 to 9.

The `bug.js` file contains the erroneous code. The `bugSolution.js` file shows the correct implementation that will generate the expected behavior.