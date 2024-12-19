# Unnecessary Re-renders in useEffect Hook
This example demonstrates a common issue when using React's `useEffect` hook.  The effect function, as written, will execute after *every* render, even if the `count` variable hasn't actually changed.

The solution involves using the dependency array (`[count]`) to specify that the effect should only run when the value of `count` changes.