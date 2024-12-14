# React Native FlatList Rendering Issue
This repository demonstrates a common issue in React Native where a FlatList component fails to render items after updating its data using useState within a useEffect hook.  The issue stems from the asynchronous nature of state updates and how they interact with the rendering process of FlatList. 

The `bug.js` file contains the problematic code. The `bugSolution.js` file provides a corrected version that ensures the FlatList correctly displays the data.

## How to reproduce
1. Clone this repository.
2. Run `npm install` to install the necessary dependencies.
3. Run `npx react-native run-android` or `npx react-native run-ios` to start the app. 
4. Observe that the FlatList is initially blank.

## Solution
The solution involves using the `items` state variable directly in the FlatList's `data` prop and the appropriate keys. Refer to `bugSolution.js` for the corrected code. 