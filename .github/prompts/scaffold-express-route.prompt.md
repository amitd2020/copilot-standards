---
name: scaffold-route
description: Generates a new Express router, controller, and registers it.
---
# Goal
Create a new Express route module.

# Rules
- Output two files: `[name].routes.js` and `[name].controller.js`.
- The router file must use `express.Router()`.
- Wrap the controller function in a `try/catch` that passes errors to `next(error)`.