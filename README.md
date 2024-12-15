# React Native FlatList Blank After API Call

This repository demonstrates a common issue in React Native where a FlatList remains blank after successfully fetching data from an API.  The issue is caused by a race condition where the component updates before the data is properly set. 

The `bug.js` file contains the buggy code. The `bugSolution.js` demonstrates the solution.

## How to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npx react-native run-android` or `npx react-native run-ios`.

## Solution

The solution is detailed in `bugSolution.js`. It addresses the race condition by checking if the data array is empty before rendering the FlatList.