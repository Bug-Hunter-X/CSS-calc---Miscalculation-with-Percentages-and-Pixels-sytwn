# CSS calc() Calculation Issue

This repository demonstrates a common issue encountered when using the `calc()` function in CSS with a combination of percentages and pixels. The problem arises from the order of operations and how the browser interprets the calculation within different contexts.

The `bug.css` file contains the erroneous CSS that causes the unexpected layout behavior. The `bugSolution.css` file shows a solution to correct the issue.

## Issue Description

The `calc()` function, while powerful, can produce unexpected results if not used carefully, especially when combining percentages and fixed units (like pixels or ems).  The main issue occurs because the browser calculates the percentages relative to the parent container's dimensions, but the fixed values are then subtracted from this percentage-based calculation.

## How to Reproduce

1. Clone this repository.
2. Open `index.html` (you'll likely need to create a simple HTML file to test the CSS).
3. Observe the unexpected layout caused by the incorrect use of `calc()`.

## Solution

The solution demonstrates how to potentially address the issue, possibly by rethinking the approach to achieve the intended layout without relying on a calculation which is easily prone to unexpected behavior in complex layouts. Different solutions may be suitable depending on the context and desired behavior.