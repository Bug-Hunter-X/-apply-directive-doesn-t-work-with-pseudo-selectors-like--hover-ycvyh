# Tailwind CSS @apply Directive Bug with Pseudo-Selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to apply styles when used with pseudo-selectors such as `:hover`, `:focus`, etc.

## Bug Description

The `@apply` directive, intended for applying pre-defined utility classes, does not correctly handle classes containing pseudo-selectors.  This leads to the styles not being applied in the expected pseudo-state. 

## Reproduction

1. Clone this repository.
2. Open `bug.html` in your browser.
3. Observe that the hover effect is missing on the button. 

## Solution

The solution involves avoiding the use of `@apply` with pseudo-selectors and applying styles directly or using JavaScript to handle the hover effect.  The `bugSolution.html` file demonstrates a working solution.

## Note

This bug highlights the limitations of using `@apply` with complex class structures and the importance of carefully considering when and how to use it.