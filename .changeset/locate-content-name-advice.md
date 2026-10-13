---
'e2e': patch
---

MCP `locate` no longer sends a role and name that match nothing back to the observation as an accessible name. It says that `observe` can show a status or alert message, or a list item, by its text, and names the `getByRole(role).filter({ hasText })` and `getByText` calls that match that text. A query that already has `exact: false` is no longer told to loosen the match with `exact: false`.
