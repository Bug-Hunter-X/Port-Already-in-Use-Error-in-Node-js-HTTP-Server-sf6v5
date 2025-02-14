# Node.js Port Already in Use Error

This repository demonstrates a common error in Node.js where attempting to start an HTTP server on a port that's already in use leads to unexpected behavior. The error message can be unclear, making debugging difficult.

## The Problem

The provided `bug.js` file starts a simple HTTP server. If you run this code while port 8080 is already occupied (e.g., by another instance of the server or a different application), it won't throw a clear and informative error.  Instead, the server might appear to start without any indication of the problem, or it might silently fail.

## The Solution

`bugSolution.js` provides a more robust way to handle the port-in-use scenario. It uses asynchronous operations and error handling to gracefully manage situations where the port is unavailable.