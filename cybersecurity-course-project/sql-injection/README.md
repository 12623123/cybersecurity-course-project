# SQL Injection Test Notes

The Bulgarian course report documents a limited set of input tests against a web application.

## Areas tested
- Login form
- “Add Stock to Portfolio” ticker-symbol field
- Dynamic URL paths containing numeric identifiers

## Observed responses in the report
- Login payloads were rejected with a standard invalid-credentials message.
- The stock-symbol field responded with “We do not support this stock”.
- Modified URL paths returned a 404 page.

These outcomes mean the documented attempts did not demonstrate successful SQL injection. They do not establish that every endpoint is secure; a broader, authorized assessment would be needed for that conclusion.

## Prevention topics
- Parameterized queries / prepared statements
- Safe ORM usage
- Input validation and type constraints
- Least-privilege database accounts
- Generic error messages that do not expose internals

## Authorization
Run tests only on systems you own or have explicit permission to assess.
