---
applyTo: "src/models/**/*.ts"
---
# MongoDB & Mongoose Rules
- Always define explicit TypeScript interfaces for Mongoose schemas.
- Disable the default `__v` version key unless document versioning is strictly required.
- Enable `timestamps: true` on all schemas to automatically track `createdAt` and `updatedAt`.