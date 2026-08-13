# Rails API Checklist

- [ ] Use `rails new --api` to skip browser assets
- [ ] Set `config.api_only = true`
- [ ] Add `gem 'rack-cors'` and configure origins
- [ ] Version your endpoints (`/api/v1/...`)
- [ ] Use `ActiveModel::Serializer` or `jsonapi-serializer`
- [ ] Keep controllers thin with service objects
- [ ] Add `skip_forgery_protection` only if needed
- [ ] Document with OpenAPI (rswag or apipie)
- [ ] Test with `rspec` + `factory_bot`
- [ ] Add rate limiting for public endpoints