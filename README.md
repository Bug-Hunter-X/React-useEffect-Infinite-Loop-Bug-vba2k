# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by a missing dependency in the dependency array. 

## Description
The `bug.js` file contains a component that increments a counter. The `useEffect` hook logs the current count to the console. However, because the `count` variable is not included in the dependency array, the effect runs on every render, causing an infinite loop and potentially crashing the application.

## Solution
The `bugSolution.js` file shows the corrected code. By adding `count` to the dependency array, the effect runs only when `count` changes, resolving the infinite loop issue.

## How to run
1. Clone this repository
2. Navigate to the repository directory
3. Run `npm install` to install dependencies
4. Run `npm start` to start the development server.