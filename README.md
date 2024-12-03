# Unhandled Null Value Access in Firebase Firestore

This repository demonstrates a common error when working with Firebase Firestore: attempting to access nested fields in a document when a parent field is null.  This can lead to unexpected errors and crashes in your application.

The `bug.js` file shows the problematic code, and `bugSolution.js` provides a corrected implementation to safely handle null values.

## How to Reproduce

1. Clone this repository.
2. Set up a Firebase project and initialize Firestore.
3. Run `bug.js` to see the error.
4. Run `bugSolution.js` to see the corrected implementation.

## Solution

The solution involves using optional chaining (`?.`) and nullish coalescing (`??`) operators (if your JavaScript version supports them), or conditional checks to ensure that you only access nested fields if the parent field is not null.