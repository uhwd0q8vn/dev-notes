# API Versioning Notes

Date: 2026-08-26

- Prefer URL path versioning for public APIs (`/v1/resource`) — simple and explicit.
- Keep deprecated versions alive long enough for clients to migrate, but set clear sunset dates.
- Use a changelog to communicate breaking changes.
- For internal APIs, consider header-based versioning to keep URLs clean.
- Always document versioning strategy in the README.
