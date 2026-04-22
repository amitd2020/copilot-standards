---
name: create-model
description: Generates a standard Mongoose schema and model.
---
# Goal
Generate a MongoDB model using Mongoose.

# Rules
- Include an exported TypeScript interface.
- Add `timestamps: true`.
- Ensure string fields that are frequently searched are marked with `index: true`.