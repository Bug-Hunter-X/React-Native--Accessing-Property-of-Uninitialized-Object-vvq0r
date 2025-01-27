# React Native: Accessing Property of Uninitialized Object

This repository demonstrates a common error in React Native applications: attempting to access a property of an object before the object has been fully initialized. This typically occurs when dealing with asynchronous operations such as data fetching.

The `bug.js` file contains code that reproduces the error, while `bugSolution.js` provides a corrected version that handles the asynchronous data loading properly.

## Error Description

The error message usually indicates that you're trying to access a property of `null` or `undefined`.  This happens because the component renders before the data has been fetched and assigned to the component's state.