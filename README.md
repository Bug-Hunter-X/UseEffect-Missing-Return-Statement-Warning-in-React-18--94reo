# React 18 useEffect Cleanup Warning

This repo demonstrates a common warning in React 18+ related to the `useEffect` hook.  The issue arises when the cleanup function is omitted from the `useEffect` hook, even if no cleanup is explicitly needed.

## The Problem

In React 18 and later, the framework provides a stricter warning when useEffect's return function is absent.  While the app may appear functional, this warning indicates a potential performance or memory leak issue if cleanup is required.

## The Solution

Always include a return statement in your `useEffect` hook, even if it's an empty function.  This ensures that React handles potential cleanup tasks effectively.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to run the application.
4. Observe the warning in the browser's developer console.