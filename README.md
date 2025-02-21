# Express.js Route Handler Error

This repository demonstrates a common error in Express.js route handlers:  missing error handling for invalid input.

The `bug.js` file contains the erroneous code.  It attempts to retrieve a user based on an ID passed in the URL parameters.  However, it lacks error handling for scenarios where the ID is not a valid integer, leading to a potential server crash or unexpected behavior.

The solution, provided in `bugSolution.js`, demonstrates proper error handling by using a `try...catch` block to handle potential `parseInt` errors and by explicitly checking if the user is found before sending the response.