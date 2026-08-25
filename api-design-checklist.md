# API Design Checklist

Useful patterns from recent Rails API work.

- Prefer plain JSON for internal APIs; JSON:API only for public, long-lived contracts.
- Version from day one: `/api/v1/...`.
- Return IDs as strings in JSON to avoid JS integer precision issues.
- Use status codes deliberately: 201 on create, 204 on delete, 422 for validation errors, 401/403 for auth.
- Include `request_id` in every response (Rails: `request.request_id`).
- Paginate with `page` / `per_page`, and include total count in `meta`.
- Keep error format consistent: `{ "error": { "code": "...", "message": "..." } }`.
- Timestamps should be ISO8601 UTC: `Time.now.utc.iso8601`.
- Don't over-serialize: expose only what the client needs.
- Document all endpoints in OpenAPI once the shape stabilizes.
