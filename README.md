# Unhandled JS Exception: Cannot read properties of null (reading 'name') in React Native

This repository demonstrates a common React Native error: 'Cannot read properties of null (reading 'name')'. This occurs when trying to access a property of an object that is null or undefined, often before asynchronous data has loaded.

## Problem
The `bug.js` file shows an example where a component tries to access the `name` property of `userData` before `fetchData()` has completed and populated `userData` with an object. This leads to the error.

## Solution
The `bugSolution.js` file provides a solution using optional chaining (`?.`) and the nullish coalescing operator (`??`).  Optional chaining safely handles null or undefined objects preventing the error. The nullish coalescing operator provides a default value if the property is null or undefined.