# React Router v6 Nested Route Issue

This repository demonstrates a common issue encountered when using nested routes in React Router v6. The problem arises from an incorrectly placed catch-all route (`/*`), which interferes with the rendering of other routes, specifically nested ones.

## Problem

The provided `App.js` shows an example where a catch-all route is defined after other routes. This causes nested routes to not render correctly because the catch-all route will always match.  

## Solution

The solution provided in `AppSolution.js` demonstrates how to resolve the problem. The catch-all route is moved to be the last route in the `Routes` component.  This ensures that it only matches routes that don't match any of the preceding more specific routes. 