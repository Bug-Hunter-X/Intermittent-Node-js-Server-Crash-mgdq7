# Intermittent Node.js Server Crash

This repository demonstrates a bug causing intermittent crashes in a simple Node.js HTTP server. The server typically runs without issue, but occasionally terminates unexpectedly without any error messages in the console.  The cause is subtle and difficult to debug using standard approaches.

## Bug

The `bug.js` file contains the problematic server code.  The crash occurs randomly, making debugging challenging.

## Solution

The solution is to add proper error handling to the server. The `bugSolution.js` file provides corrected code which handles potential errors gracefully.

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository directory.
3. Run `node bug.js`.
4. Observe the server output and whether it crashes after some time of running.
5. Repeat steps 3 and 4 to increase likelihood of observing the crash.

## Note

The intermittent nature of this bug makes it difficult to pinpoint with conventional debugging methods.  This example highlights the importance of comprehensive error handling in production Node.js applications.