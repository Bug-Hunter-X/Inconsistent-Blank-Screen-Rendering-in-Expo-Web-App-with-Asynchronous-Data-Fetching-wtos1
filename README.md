# Inconsistent Blank Screen Rendering in Expo Web App with Asynchronous Data Fetching

This repository demonstrates a bug encountered when using the Expo Web SDK and navigating to screens with asynchronous data fetching.  The problem is characterized by inconsistent rendering of blank screens, even when data eventually loads successfully. The issue is more prevalent when using asynchronous operations within useEffect hooks.

## Reproducing the Bug

Follow the steps below to attempt to reproduce the issue:
1. Clone this repository.
2. Navigate to the project directory: `cd expo-routing-bug`
3. Install dependencies: `npm install` or `yarn install`
4. Start the development server: `expo start`
5. Navigate between screens.  The blank screen might not always occur, but inconsistent rendering should be noticeable.

## Potential Solutions

See `bugSolution.js` for a potential solution involving better handling of asynchronous data fetching and the use of loading states.