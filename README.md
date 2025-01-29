# CSS Specificity Bug: Unexpected Background Color Inheritance

This repository demonstrates a subtle CSS specificity issue.  Despite applying a more specific style to a nested `<p>` element within a `.container`, the expected background color doesn't always override the less specific style. This highlights potential inconsistencies across different browsers.

## The Problem

The `bug.css` file contains CSS that unexpectedly inherits a background color. The `lightgreen` background should override `lightcoral` due to the higher specificity of `.container p`, but this isn't always guaranteed in practice.

## The Solution

The `bugSolution.css` file demonstrates a solution to this. It applies !important to the `.container p` style to force the override, ensuring consistent behavior across browsers.