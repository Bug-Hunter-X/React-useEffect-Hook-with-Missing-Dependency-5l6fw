# React useEffect Hook with Missing Dependency

This repository demonstrates a common bug in React involving the `useEffect` hook and its dependency array.  The example shows how omitting a necessary dependency can lead to an infinite render loop and unexpected behavior.  The solution shows the correct way to use `useEffect` with the correct dependencies.

**Bug:** The initial example has a `useEffect` hook that logs the current count to the console. However, the `count` variable is missing from the dependency array. This causes the effect to run after every render, creating an infinite loop and excessive console logs. 

**Solution:** The solution includes adding `count` to the dependency array. This ensures the effect only runs when the `count` variable changes, preventing the infinite loop.