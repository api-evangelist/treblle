---
name: treblle-list-and-invite-members
description: Retrieve the current project members and then invite a new member to the project.
api: openapi/treblle-members-api-openapi.yml
operations:
- listMembers
- inviteMember
generated: '2026-10-04'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/treblle-members-api-openapi.yml ; every operationId checked against the contract
---

# treblle-list-and-invite-members

Retrieve the current project members and then invite a new member to the project.

## Steps

1. 1. Call `listMembers` with optional pagination query parameters (`offset`, `limit`, `page`, `per_page`) and include the `Treblle-Api-Key` header.
2. 2. Call `inviteMember` with the required request body fields for the new member and include the `Treblle-Api-Key` header.

## Rules

- Auth: Provide the API key in the `Treblle-Api-Key` request header.
- Pagination: `listMembers` supports `offset`, `limit`, `page`, and `per_page` query parameters.
- Errors: On rate‑limit exhaustion the API returns no specific HTTP status code (HTTP None).
