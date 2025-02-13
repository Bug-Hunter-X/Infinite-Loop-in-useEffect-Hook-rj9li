# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications: creating an infinite loop within the `useEffect` hook.

## Bug Description

The `MyComponent` component uses `useState` to track a count.  The `useEffect` hook attempts to increment this count, but because 'count' is in the dependency array, the effect runs again, causing a loop that never ends and crashes the application.

## Solution

The solution involves carefully managing dependencies to prevent the infinite loop.