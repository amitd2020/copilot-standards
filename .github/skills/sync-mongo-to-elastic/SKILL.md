# Sync MongoDB to Elasticsearch
Trigger this skill when asked to write data synchronization scripts or Mongoose middleware.

## Workflow
1. **Analyze:** Look at the provided Mongoose schema.
2. **Strategy:** Propose a Mongoose `post('save')` and `post('remove')` hook strategy to push changes to the Elasticsearch index automatically.
3. **Drafting:** Write the synchronization logic using the official `@elastic/elasticsearch` Node client. Ensure bulk indexing is used if the user asks for a seeding script.