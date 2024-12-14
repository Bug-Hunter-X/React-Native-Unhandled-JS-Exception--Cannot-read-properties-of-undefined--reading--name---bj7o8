# React Native Unhandled JS Exception: Cannot read properties of undefined (reading 'name')

This repository demonstrates a common React Native error: "Cannot read properties of undefined (reading 'name')" and provides a solution.

The error occurs when attempting to access a property of an object before the object is fully initialized, often due to asynchronous operations like data fetching.  The provided code examples showcase the problem and its solution using conditional rendering and optional chaining.

## Problem

The provided `bug.js` file shows a React Native component that fetches data asynchronously.  It attempts to access the `name` property of the `data` object immediately, before the data has been fetched and set.  This leads to the "Cannot read properties of undefined (reading 'name')" error.

## Solution

The `bugSolution.js` file demonstrates how to solve the problem using conditional rendering and optional chaining.  Conditional rendering prevents the component from attempting to access properties until the data is available. Optional chaining safely handles cases where the data might still be undefined.