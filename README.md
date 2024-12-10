# React Native: Handling Asynchronous State Updates

This repository demonstrates a common error in React Native applications: accessing a state variable before it's been initialized after an asynchronous operation. The `bug.js` file shows the problematic code where `data.name` is accessed before the API call in `useEffect` completes.  The solution, provided in `bugSolution.js`, shows how to correctly handle this using optional chaining and/or nullish coalescing to avoid the error.  This ensures a more robust and reliable application that gracefully handles potential undefined values.

## How to reproduce the bug:
1. Clone this repository.
2. Run `npm install`.
3. Run the application (e.g., with Expo).
4. Observe the error in the console.