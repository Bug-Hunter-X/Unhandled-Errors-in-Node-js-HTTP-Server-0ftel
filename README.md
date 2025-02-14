# Unhandled Errors in Node.js HTTP Server

This repository demonstrates a common error in Node.js applications: improper error handling in HTTP servers. The initial `server.js` example lacks error handling, making it vulnerable to crashes. The improved `serverSolution.js` provides a robust solution.

## Problem

The original code creates an HTTP server but fails to handle potential errors during the request handling process. This can lead to unexpected crashes and downtime.

## Solution

The solution implements proper error handling within the `requestListener` function.  It includes a `try...catch` block to gracefully handle any exceptions that might occur during request processing.  This prevents the server from crashing and allows for more controlled error management.

## Usage

1. Clone this repository.
2. Run `node server.js` (original code with error). Observe that it doesn't handle errors.
3. Run `node serverSolution.js` (corrected code). Observe that errors are handled gracefully.