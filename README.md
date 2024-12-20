# React useEffect Dependency Array Bug

This repository demonstrates a common bug in React's `useEffect` hook:  forgetting to include state variables in the dependency array. This leads to unexpected behavior and possibly infinite renders. 

The `bug.js` file contains the buggy code. The `bugSolution.js` file provides the corrected implementation.

## Bug
The original code lacks the `count` variable in the dependency array, causing the effect to run on every render regardless of changes to the count.