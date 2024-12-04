# CSS Specificity Conflicts

This repository demonstrates a common issue encountered when working with CSS: unexpected style application due to specificity conflicts.  Inline styles often override internal stylesheets, making debugging difficult. The `bug.css` file contains the buggy code. The `bugSolution.css` file shows how to solve this.

## Problem
Inline styles have higher specificity than most other styles, even if those other styles are more 'specific' in their selectors. This can lead to unintentional styling overrides. 

## Solution
Use more specific selectors in your internal stylesheets to override inline styles. Be very mindful of the cascade and specificity rules.  It is often better to avoid inline styles altogether unless absolutely necessary.