# Unresponsive Node.js Server

This repository demonstrates a common issue in Node.js: an unresponsive server caused by a long-running synchronous operation blocking the event loop.  The `bug.js` file contains code that simulates this problem.  The solution (`bugSolution.js`) shows how to address this using asynchronous programming.

## How to Reproduce

1. Clone this repository.
2. Run `node bug.js`.
3. Try to access `http://localhost:3000/` in your browser. You'll notice the response is very slow or the server appears unresponsive.

## Solution

The solution involves using asynchronous operations (like promises or async/await) to avoid blocking the event loop.  The `bugSolution.js` file provides an example of how to refactor the code for improved responsiveness.