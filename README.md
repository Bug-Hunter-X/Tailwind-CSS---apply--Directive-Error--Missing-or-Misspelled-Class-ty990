# Tailwind CSS `@apply` Directive Error: Missing or Misspelled Class

This repository demonstrates a common yet subtle error when using Tailwind CSS's `@apply` directive.  The issue arises when attempting to apply a class that is either misspelled or not defined in your Tailwind configuration.

## The Problem

The `@apply` directive provides a convenient way to reuse styles.  However, if the class you're applying doesn't exist, Tailwind won't throw an error; instead, it will silently fail to apply any styles. This can lead to debugging headaches as the issue isn't immediately apparent.

## Reproduction

1. Clone this repository.
2. Open `bug.html` in your browser.  You'll notice the div doesn't have the expected red background.
3. Open `bugSolution.html` to see the corrected version.

## Solution

The solution is straightforward: double-check the spelling of your class names and ensure they're correctly defined in your `tailwind.config.js` file (or your equivalent configuration file).  Use your IDE's autocompletion features to help prevent typos.