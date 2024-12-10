# React Router v6 Catch-All Route Issue

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router v6. The problem is that the catch-all route is not working as intended, leading to errors instead of the expected 404 page.

## Bug Description
The provided `App.js` file contains a simple React application using React Router v6.  Despite the inclusion of a `/*` catch-all route, accessing non-existent paths results in an error rather than rendering the `NotFound` component as expected. 

## Solution
The solution, in `AppSolution.js`, addresses the issue by ensuring the catch-all route is correctly positioned within the `Routes` component. The order of routes matters in React Router v6; the catch-all route must be the last one defined to function correctly. 