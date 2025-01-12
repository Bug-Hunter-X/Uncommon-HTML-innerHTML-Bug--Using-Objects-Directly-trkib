# Uncommon HTML innerHTML Bug: Using Objects Directly

This repository demonstrates a subtle bug related to the `innerHTML` property in HTML and JavaScript.

The bug is caused by attempting to directly assign a JavaScript object to the `innerHTML` property of a DOM element.  Instead of rendering the object's contents, this results in an empty or unexpected output.

## Bug Description
The `bug.html` file contains the erroneous code.  It attempts to set the `innerHTML` of a div element to a JavaScript object. This does not work as expected and produces an empty div instead of displaying the object's contents.

## Solution
The `solution.html` file demonstrates the corrected approach. To display the object's data, you must first convert it to a string representation using JSON.stringify().