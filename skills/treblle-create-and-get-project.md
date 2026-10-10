---
name: treblle-create-and-get-project
description: Create a new project and then retrieve its details.
api: openapi/treblle-projects-api-openapi.yml
operations:
- createProject
- getProject
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/treblle-projects-api-openapi.yml ; every operationId checked against the contract
---

# treblle-create-and-get-project

Create a new project and then retrieve its details.

## Steps

1. 1. Use `createProject` with the request body containing the project data and include the header `Treblle-Api-Key`.
2. 2. Use `getProject` with the path parameter `projectId` returned from the previous step and include the header `Treblle-Api-Key`.

## Rules

- Auth: Include the `Treblle-Api-Key` header for all requests.
- Idempotency: Not applicable for these operations.
- Pagination: Not applicable for this task.
