# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling when dealing with user input.  Specifically, the example shows a route that retrieves a user by ID.  The code fails to handle cases where the provided ID is not a valid integer, potentially leading to application crashes or unexpected behavior.

## Bug

The `bug.js` file contains the erroneous code.  It attempts to parse the user ID as an integer without validating that it's a number, which can result in an error if the ID is non-numeric.

## Solution

The `bugSolution.js` file demonstrates the corrected code with improved error handling.  It includes a check to ensure the ID is a valid integer before attempting to parse it. If the ID is invalid, an appropriate error message is returned.