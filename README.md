# Next.js 15 Unhandled Runtime Error: Cannot read properties of undefined (reading 'name')

This repository demonstrates a common runtime error in Next.js 15 applications where accessing a property of an undefined prop causes the application to crash.

## The Problem

The `About` component attempts to access the `name` property of the `data` prop. If `data` is undefined, this will throw a runtime error.  This is common in situations where data fetching or prop passing is not handled correctly.

## The Solution

The solution involves adding a check to ensure that `data` is defined before attempting to access its `name` property.  Optional chaining and nullish coalescing are ideal for concise handling.

## Reproduction

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to `/about`.  You'll see the error in your browser console.

## How to fix

Review the code in `aboutSolution.js` for a corrected implementation.