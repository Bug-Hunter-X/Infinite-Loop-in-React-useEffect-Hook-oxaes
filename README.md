# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug: an infinite loop caused by incorrect usage of the `useEffect` hook.

## Bug Description
The `bug.js` file contains a component that uses the `useEffect` hook to update the state.  However, the dependency array is empty (`[]`), causing the effect to run repeatedly, resulting in an infinite loop and crashing the application. 

## Solution
The `bugSolution.js` file demonstrates the correct way to use the `useEffect` hook. By adding the `count` variable to the dependency array (`[count]`), the effect only runs when the value of `count` changes.  This prevents the infinite loop.

## How to Reproduce
1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the application.
4. Observe the infinite loop in the browser's console.
5. Uncomment the corrected useEffect in `bugSolution.js` to see the working solution.