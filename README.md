# Node.js Server - Port Already in Use

This repository demonstrates a common Node.js error: 'Error: listen EADDRINUSE: address already in use :::8080'.  This occurs when attempting to start a server on a port that is already being used by another process.

## Bug

The `bug.js` file contains a simple HTTP server that attempts to listen on port 8080. If another application is already using this port (e.g., another Node.js server or a different service), the server will fail to start.

## Solution

The `bugSolution.js` file provides a solution. It uses the `process.exit()` method to gracefully handle the error and exit the process when the port is unavailable, preventing the application from hanging.