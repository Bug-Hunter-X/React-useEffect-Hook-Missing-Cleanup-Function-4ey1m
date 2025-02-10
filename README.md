# React useEffect Hook Missing Cleanup Function

This repository demonstrates a common error in React applications: forgetting to include a cleanup function in the `useEffect` hook. This can lead to memory leaks and unexpected behavior.

The `bug.js` file contains the erroneous code.  The `bugSolution.js` file provides the corrected code.

## Bug Description

The `useEffect` hook in `bug.js` lacks a return statement. This return statement is crucial for cleaning up resources when the component unmounts or updates. Without it, any side effects (like subscriptions or timers) will continue running, potentially leading to performance issues or memory leaks. 

## Solution

The `bugSolution.js` file shows the corrected code. The added return statement ensures that the console log is cleared when the component is unmounted. This is a fundamental aspect of managing side effects within React components. 