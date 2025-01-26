# React 19 useEffect Bug

This repository demonstrates a common bug in React 19 involving the `useEffect` hook and its dependency array.

## Bug Description
The bug is caused by omitting a state variable from the `useEffect` dependency array, leading to an infinite render loop.

## How to Reproduce
1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console output and notice the component re-renders infinitely.

## Solution
The solution involves correctly specifying the state variable (`count` in this case) in the dependency array. This ensures the effect only runs when the state variable changes.

## Additional Notes
This example highlights the importance of correctly managing dependencies in `useEffect` hooks to avoid performance issues and unexpected behavior.