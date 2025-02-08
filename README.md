# Infinite useEffect Loop in React

This repository demonstrates a common React bug: an infinite loop caused by an incorrectly used `useEffect` hook. The `useEffect` hook, while powerful, can easily lead to performance problems if not used correctly. This example shows a typical scenario and provides a solution. 

## Problem

The `bug.js` file contains a component that uses `useEffect` to log the count. However, the effect is called on every render because there are no dependencies passed to the useEffect hook causing an infinite loop.

## Solution

The `bugSolution.js` file shows how to fix the problem by correctly specifying dependencies for the useEffect hook, ensuring the effect runs only when the `count` changes.