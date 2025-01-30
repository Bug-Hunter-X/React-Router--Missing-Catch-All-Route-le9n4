# React Router: Missing Catch-All Route

This repository demonstrates a common issue in React Router v6:  failure to include a catch-all route (`/*`) to handle paths not explicitly defined.  Without a catch-all, accessing an undefined route results in a blank page or unexpected behavior.

The `App.js` file shows the buggy code; `AppSolution.js` provides the solution.

## Problem:
When navigating to a URL that doesn't have a corresponding Route, the app silently fails.  In development, you might see an error message, but in production, it will result in a blank screen or unpredictable behavior.

## Solution:
Adding a `Route` with the path `/*` as a catch-all to handle any unexpected URLs prevents this issue.  You can typically handle this by displaying a 404 Not Found page or redirecting to a default route.