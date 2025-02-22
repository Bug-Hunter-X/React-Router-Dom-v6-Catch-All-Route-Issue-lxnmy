# React Router Dom v6 Catch-All Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router v6. The catch-all route is unexpectedly triggered even when other routes should match.

## Bug Description

The provided `App.js` file contains a simple React Router setup.  The `/*` catch-all route is intended to handle any unmatched routes. However, it's always triggered, even when a route like `/` or `/about` should match.  This causes the 404 page to always display, even when the user is on valid routes.

## Solution

The solution in `AppSolution.js` demonstrates how to correctly structure the routes to prevent this behavior.  The order of routes matters.  The catch all route should be defined last. 

## Setup

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.