# Express.js Unhandled Database Error

This repository demonstrates a common error in Express.js applications: missing error handling for database operations within route handlers.

The `bug.js` file showcases a route that fetches user data from a database.  It correctly handles the case where a user is not found (404). However, it lacks error handling for potential database issues like connection errors or query failures.  This can lead to server crashes or unexpected behavior.

The `bugSolution.js` file provides a corrected version with robust error handling, demonstrating best practices for handling database-related errors in Express.js routes.  It uses `try...catch` blocks to gracefully handle potential exceptions and sends appropriate error responses to the client.