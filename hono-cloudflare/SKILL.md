# Hono + Cloudflare Workers Skill

Build robust, scalable, and maintainable backend services using Hono and Cloudflare Workers.

## Core Principles

* Follow the existing project architecture, conventions, and Cloudflare configuration.
* Prefer Cloudflare Workers-native APIs and services over Node.js-specific APIs.
* Keep handlers small, focused, and easy to test.
* Separate routing, business logic, validation, and data access when appropriate.
* Prefer simple solutions over unnecessary abstractions.
* Reuse existing utilities, middleware, schemas, and services.

## Hono

* Use Hono routing and middleware consistently.
* Keep route handlers focused on HTTP concerns.
* Use Hono context (`c`) correctly for request, response, environment bindings, and variables.
* Prefer middleware for cross-cutting concerns such as authentication, logging, CORS, and error handling.
* Validate request parameters, query strings, headers, and bodies before using them.
* Return appropriate HTTP status codes and consistent response formats.
* Keep API error responses predictable and useful.
* Avoid putting complex business logic directly inside route handlers.

## Cloudflare Workers

* Follow the Workers runtime model and avoid Node.js-only APIs.
* Use `env` bindings for environment variables, secrets, KV, R2, D1, Durable Objects, Queues, and other Cloudflare services.
* Never hardcode secrets, API keys, tokens, or credentials.
* Prefer asynchronous APIs and avoid blocking operations.
* Consider Worker execution limits and request lifecycle when designing backend logic.
* Use `waitUntil()` for non-critical background work when appropriate.
* Handle external API failures, timeouts, and unexpected responses safely.

## Environment and Bindings

* Inspect `wrangler.jsonc`, `wrangler.toml`, or existing Cloudflare configuration before changing bindings.
* Reuse existing bindings instead of creating duplicates.
* Keep local, preview, and production environments clearly separated.
* Do not modify Cloudflare configuration unless required by the task.
* Ensure new bindings are correctly typed in the project's environment types.

## API Design

* Use consistent URL patterns and HTTP methods.
* Validate all external input.
* Return clear and predictable JSON responses.
* Use proper status codes for success, validation errors, authentication failures, authorization failures, not-found cases, conflicts, and server errors.
* Avoid leaking internal errors, secrets, stack traces, or implementation details.
* Design APIs to be backward-compatible when possible.

## Security

* Treat all client input as untrusted.
* Validate and sanitize input at the API boundary.
* Authenticate and authorize protected endpoints.
* Never expose secrets or sensitive environment variables in responses.
* Protect against common API issues such as injection, broken authorization, excessive payloads, and abuse.
* Configure CORS deliberately instead of allowing unrestricted origins unless required.
* Apply rate limiting or Cloudflare-native protection when appropriate.

## Database and Storage

* Reuse existing database and storage patterns.
* Use D1 for relational data, KV for simple key-value data, R2 for object storage, and Durable Objects for stateful coordination when appropriate.
* Avoid unnecessary database queries.
* Use parameterized queries.
* Handle transactions and concurrent updates correctly.
* Consider indexes and query performance when working with D1.

## External APIs

* Validate external API responses instead of assuming their structure.
* Handle timeouts, rate limits, retries, and transient failures appropriately.
* Avoid unnecessary external requests.
* Do not expose third-party credentials to clients.
* Keep external API integrations isolated from route handlers when practical.

## Error Handling

* Use centralized error handling when the project supports it.
* Return consistent error responses.
* Log useful diagnostic information without logging secrets or sensitive data.
* Distinguish expected client errors from unexpected server errors.
* Never silently ignore failures.

## Implementation Rules

* Inspect existing routes, middleware, services, schemas, and bindings before implementing changes.
* Search for similar endpoints and reuse established patterns.
* Make the smallest necessary changes.
* Avoid unrelated refactoring.
* Do not invent Cloudflare bindings, APIs, or runtime capabilities.
* Check the installed versions of Hono, Wrangler, and relevant Cloudflare packages before using newer APIs.
* Prefer existing project dependencies over adding new ones.
* Keep types accurate and avoid `any`.

## Verification

After making changes, run available checks such as:

* TypeScript type checking
* Linting
* Unit or integration tests
* Wrangler validation
* Build or deployment checks when appropriate

Verify both successful and failure paths for API changes.

## Avoid

* Node.js APIs that are unavailable in the Workers runtime.
* Hardcoded secrets or credentials.
* Unvalidated request data.
* Business logic scattered across route handlers.
* Unnecessary middleware.
* Unnecessary database queries.
* Unnecessary external API calls.
* Catching errors without handling or logging them.
* Large architectural changes for small feature requests.
