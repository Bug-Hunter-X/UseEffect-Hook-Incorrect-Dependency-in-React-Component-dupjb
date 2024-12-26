# React useEffect Hook Incorrect Dependency

This repository demonstrates a common error in React's `useEffect` hook: incorrect dependency handling. The component's title should update whenever the `count` changes, but the current implementation only updates it when `count` is 0.

## Bug

The `bug.js` file contains the buggy code. The `useEffect` hook only updates the document title when the `count` is 0. When the count is incremented, the title does not change.

## Solution

The `bugSolution.js` file provides a corrected version. The dependency array in `useEffect` is fixed to include `count`, causing the title to update every time the `count` changes.