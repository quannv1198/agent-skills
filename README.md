# AI Coding Skills

Skills for AI coding agents.

## Base URL

```text
https://raw.githubusercontent.com/quannv1198/agent-skills/refs/heads/master
```

## Available Skills

### React Coding


```text
Path: /react-coding/SKILL.md
```

Purpose:
Helps AI write clean, reusable, performant, and maintainable React code while following existing project patterns and conventions.

---

### TypeScript


```text
Path: /typescript/SKILL.md
```

Purpose:
Helps AI write type-safe and maintainable TypeScript code, avoid unsafe typing, and follow existing TypeScript conventions.

---

### Code Review


```text
Path: /code-review/SKILL.md
```

Purpose:
Helps AI review code for bugs, security issues, performance problems, maintainability, and overall code quality.

---

### UI Design


```text
Path: /ui-design/SKILL.md
```

Purpose:
Helps AI build polished, modern, consistent, and user-friendly interfaces with strong visual hierarchy, spacing, typography, responsive layouts, accessibility, and interaction design.

---

### Hono + Cloudflare Workers


```text
Path: /hono-cloudflare/SKILL.md
```

Purpose:
Helps AI build robust and maintainable backend APIs using Hono and Cloudflare Workers, following Workers runtime constraints, Cloudflare services, API design, security, validation, and performance best practices.

## Skill URL

Combine `Base URL` with a skill `Path`.

```text
{BASE_URL}{PATH}
```

## Skill Selection

Use the appropriate skill based on the task:

* React component, UI, hooks, or React architecture → `react-coding`
* TypeScript types, interfaces, generics, or type safety → `typescript`
* Code auditing, debugging, or quality review → `code-review`
* UI layout, visual design, styling, responsive design, typography, accessibility, or user experience → `ui-design`
* Hono routes, middleware, API endpoints, or Hono architecture → `hono-cloudflare`
* Cloudflare Workers, D1, KV, R2, Durable Objects, Queues, bindings, or Workers runtime → `hono-cloudflare`

Multiple skills can be loaded when a task requires them.

## Instructions for AI Agents

1. Read this README to discover available skills.
2. Select the skills relevant to the current task.
3. Fetch the corresponding `SKILL.md` using the Base URL and Path.
4. Follow the loaded skill instructions when completing the task.
5. Load multiple skills when their responsibilities overlap.
6. Do not load unrelated skills unnecessarily.
