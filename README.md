# AI Coding Skills

Skills for AI coding agents.

## Base URL

```text
https://your-skill-host.com/skills
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

## Skill URLs

Combine `Base URL` with a skill `Path`.

```text
{BASE_URL}{PATH}
```

## Skill Selection

Use the appropriate skill based on the task:

* React component, UI, hooks, or React architecture → `react-coding`
* TypeScript types, interfaces, generics, or type safety → `typescript`
* Code auditing, debugging, or quality review → `code-review`

Multiple skills can be loaded when a task requires them.

## Instructions for AI Agents

1. Read this README to discover available skills.
2. Select the skills relevant to the current task.
3. Fetch the corresponding `SKILL.md` using the Base URL and Path.
4. Follow the loaded skill instructions when completing the task.
5. Load multiple skills when their responsibilities overlap.
6. Do not load unrelated skills unnecessarily.
