# Tailwind CSS @apply Directive Failure with Complex Custom Classes

This repository demonstrates an uncommon bug in Tailwind CSS related to the `@apply` directive and custom utility classes that contain variables or complex selectors. The bug manifests as unexpected styling behavior or the complete absence of styles.

## Bug Description
When using `@apply` with custom classes that involve variables or complex CSS selectors, Tailwind CSS's compilation process may fail to correctly resolve these values. This might be due to improper variable definitions, incorrectly formatted selectors, or interactions with other parts of your Tailwind configuration.

## Reproduction
1. Clone this repository.
2. Run `npm install` (assuming you have Node.js and npm installed).
3. Start a local web server to view the styles (e.g., using `python -m http.server`).
4. Observe the unexpected rendering in the browser.

## Solution
The solution involves carefully reviewing and simplifying your custom utility classes and their definitions. Ensure that variables are properly defined and accessible in the context of the custom classes, and carefully validate all selectors to avoid syntax errors.

## Further investigation
The root cause of the issue can sometimes be tracked down to interactions with other plugins or customizations within your Tailwind configuration. Thorough investigation and careful analysis of the error messages provided by the Tailwind compiler are helpful for pinpointing these problems.