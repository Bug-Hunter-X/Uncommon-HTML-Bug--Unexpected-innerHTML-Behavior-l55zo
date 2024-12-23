# Uncommon HTML Bug: Unexpected innerHTML Behavior

This repository demonstrates an uncommon bug related to the usage of `innerHTML` in HTML.  The bug arises from an incorrect understanding of how `innerHTML` handles assignments and string concatenation.

The `bug.html` file showcases the problem.  The `bugSolution.html` provides a corrected version.

## Bug Description
The bug stems from attempting to directly append text to a numerical `innerHTML` value.  The initial assignment sets `innerHTML` to the number 123.  Subsequent attempts to add strings using `+=` will concatenate the strings to the number, creating a string value, not appending a text node to the original content.