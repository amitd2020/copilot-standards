# Build Fuzzy Search API
Trigger when asked to create a search endpoint that queries Elasticsearch.

## Workflow
1. **Query Construction:** Construct an Elasticsearch query that searches across multiple fields (e.g., `companyName`, `tradingNames`, `directors`). Include `fuzziness: "AUTO"`.
2. **Controller Logic:** Write an Express controller that extracts the search term from `req.query.q`, executes the Elasticsearch query, and maps the `hits.hits` array into a clean JSON array for the client response.