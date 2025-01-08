# Express.js Route Handler Bug: Missing Error Handling

This repository demonstrates a common error in Express.js route handlers:  lack of error handling for invalid input.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides the corrected version.

**Problem:**
The original code attempts to parse a user ID from the request parameters and uses it to find a user in an array. It lacks error handling for cases where the user ID is not a valid number, which could lead to unexpected crashes or incorrect responses. 

**Solution:**
The corrected code adds error handling to check if the `userId` is a number. If not, it returns an appropriate error response.  This prevents unexpected errors and improves the application's robustness.