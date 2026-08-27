# API Versioning Notes

- Prefer URL versioning (`/v1/...`) for simple, explicit versions.
- Consider header or media-type versioning for non-breaking changes.
- Never break existing clients without a deprecation cycle.
- Use semantic versioning for the API itself.
- Document deprecated endpoints and provide migration guides.
