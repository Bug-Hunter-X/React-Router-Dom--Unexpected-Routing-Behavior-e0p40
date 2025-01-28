# React Router Dom: Unexpected Routing Behavior

This repository demonstrates a common issue encountered when using React Router Dom v6: unexpected routing behavior when adding a new route. The application does not render anything when navigating to a path that doesn't have a defined route.

## Issue Description

The provided code has a `Routes` component from `react-router-dom`.  If you navigate to a path that is not explicitly defined within the `Routes` component, the application does not render anything.  This behavior is usually unexpected as it could lead to a blank screen. 

## Solution

Adding a catch-all route (`/*`) with a default component to render solves the problem. If no other route matches, this catch-all route will handle it. This could involve rendering a 404 page or redirecting to a default route.

## How to reproduce

1. Clone the repo
2. Run `npm install`
3. Run `npm start`
4. Navigate to `/contact` - the app renders nothing. 
5. See the solution in `AppSolution.js` to fix this.
