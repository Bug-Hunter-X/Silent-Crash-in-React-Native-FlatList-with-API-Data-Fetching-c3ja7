# Silent Crash in React Native FlatList with API Data Fetching

This repository demonstrates a common yet subtle bug in React Native applications involving FlatList and API data fetching.  The app crashes silently without providing any error messages on the UI when there is an issue fetching data.

The bug is reproduced in `DataList.js` and a solution is proposed in `DataListSolution.js`.

## Bug Description
The application fetches data from a public API.  If the API request fails, the app crashes without displaying an error message or providing any indication of the failure to the user. This is a poor user experience.

## How to Reproduce
1. Clone this repository.
2. Run the application in your React Native environment.
3. Observe the behavior when the API request is successful and when the API request fails. 

## Solution
The solution in `DataListSolution.js` addresses the issue by properly handling potential errors during the asynchronous API call using try...catch blocks and updating the UI accordingly to inform the user about any errors.