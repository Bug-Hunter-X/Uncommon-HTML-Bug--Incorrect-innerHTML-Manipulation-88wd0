# Uncommon HTML Bug: Incorrect innerHTML Manipulation

This repository demonstrates an uncommon bug related to the manipulation of the `innerHTML` property in HTML.  The bug is subtle but can lead to unexpected behavior or security vulnerabilities if not handled correctly.  The example shows appending to innerHTML without proper escaping, a common mistake leading to unexpected results. The solution uses DOM manipulation methods for cleaner and safer manipulation.  This approach helps prevent Cross-Site Scripting (XSS) vulnerabilities and improves code readability and maintainability.

## Bug

The `bug.html` file shows incorrect usage of innerHTML. Appending directly to `innerHTML` can cause unexpected results and security risks if the added content is not properly sanitized. 

## Solution

The `solution.html` file demonstrates the correct approach, using `insertAdjacentHTML` which offers improved control and avoids the pitfalls of direct `innerHTML` manipulation. It also provides the best practice of escaping the added text.