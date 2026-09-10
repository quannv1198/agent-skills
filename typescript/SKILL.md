# TypeScript Coding Skill

- Use strict, type-safe TypeScript.
- Prefer explicit types for public APIs, function parameters, and complex data structures.
- Avoid `any`; use `unknown` when the type is genuinely unknown.
- Prefer type inference for simple local variables.
- Use interfaces or type aliases consistently with existing project conventions.
- Reuse existing types instead of duplicating definitions.
- Use discriminated unions for state and variant-based logic when appropriate.
- Handle `null` and `undefined` explicitly.
- Avoid unsafe type assertions (`as`) unless necessary and justified.
- Prefer type guards over casting.
- Use generics when they improve type safety and reusability.
- Keep types simple, readable, and close to where they are used.
- Avoid over-engineering types for simple code.
- Preserve existing TypeScript configuration and project conventions.
- Run TypeScript checks, lint, tests, or build after significant changes when available.