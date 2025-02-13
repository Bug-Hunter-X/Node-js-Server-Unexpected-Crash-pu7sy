# Node.js Server Unexpected Crash

This repository demonstrates a bug where a Node.js HTTP server crashes unexpectedly after handling a certain number of requests. The server doesn't provide any error messages in the console, making debugging difficult.

## Bug Description
A simple HTTP server is implemented using Node.js's `http` module. Under normal circumstances, the server should continuously listen for incoming requests and respond with 'Hello, World!'. However, after handling a number of requests (this number can vary), the server crashes without any error messages being logged to the console.

## Bug Solution
The issue was resolved by implementing proper error handling using the 'error' event listener on the server object. This allows capturing the error and logging it to the console for debugging purposes. In this case, the crash is simulated, and the error handling prevents the crash.