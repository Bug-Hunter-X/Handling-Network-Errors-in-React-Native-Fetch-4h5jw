# Handling Network Errors in React Native Fetch

This example demonstrates how to robustly handle network errors when fetching data in a React Native application using the `fetch` API.  Improper error handling can lead to crashes or confusing user experiences.

## Problem

The provided `DataFetch.js` code fetches data from an API.  However, it lacks proper error handling, making the app susceptible to crashes or displaying unhelpful messages when network requests fail.

## Solution

The `DataFetchSolution.js` file provides a solution incorporating a `try...catch` block within the `useEffect` hook. This allows the application to catch network errors (HTTP errors or other issues), display an error message, and prevent app crashes. The `finally` block ensures that the loading state is always updated, regardless of success or failure.

## Usage

Clone this repository and run:
```bash
npm install
npm start
```
Then you can compare the original buggy code with the improved version that effectively manages network errors.