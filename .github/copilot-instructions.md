# Express.js API Standards
- **Syntax:** Strict ES Modules (`import`/`export`). No `require()`.
- **Async Logic:** Always use `async/await`. Never use `.then().catch()` chains or legacy callbacks.
- **Error Handling:** Controllers must never send `res.status(500)` directly. All errors must be passed to `next(error)` so they can be caught by our global Express error-handling middleware.
- **Responses:** All API responses must follow the format: `{ success: boolean, data: any, error?: string }`.