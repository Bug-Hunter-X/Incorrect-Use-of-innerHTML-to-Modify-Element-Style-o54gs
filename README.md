# Incorrect Use of innerHTML to Modify Element Style
This repository demonstrates an uncommon bug in HTML related to incorrectly using innerHTML to modify the style of an element.  The issue lies in attempting to change the display style of an element using innerHTML, which is generally used for changing the content of an element, not its style.

## Bug Description
The code uses `innerHTML` to set the style attribute of a div element to `display:none;`.  This approach is flawed because it replaces the entire content of the div, including any event listeners or other attributes, which can lead to unexpected behavior.

## Solution
The correct approach is to use `element.style.property = value;` to modify element styles directly.
