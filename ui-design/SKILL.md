# UI Design Skill

Build polished, modern, consistent, and user-friendly interfaces.

## Core Principles

* Follow the existing design system, visual language, and component patterns.
* Prefer simple, clean, intentional designs over unnecessary decoration.
* Prioritize usability, clarity, consistency, and visual hierarchy.
* Avoid generic "AI-generated" looking interfaces.
* Do not introduce a new visual style when the project already has an established one.
* Reuse existing components, tokens, and utilities whenever possible.

## Layout

* Use a consistent spacing system.
* Maintain clear alignment and visual rhythm.
* Use appropriate content width and whitespace.
* Establish a clear hierarchy between sections, headings, content, and actions.
* Avoid overcrowded layouts.
* Keep related elements visually grouped.
* Use responsive layouts that work well across mobile, tablet, and desktop.

## Typography

* Use the project's existing typography system.
* Establish clear hierarchy between headings, body text, labels, and supporting text.
* Use readable font sizes and line heights.
* Avoid excessive font weights, sizes, or decorative typography.
* Keep text lengths and wrapping in mind when designing layouts.

## Colors

* Use the existing color palette and design tokens.
* Maintain sufficient contrast between text and backgrounds.
* Use accent colors intentionally for actions, status, and emphasis.
* Do not introduce unnecessary colors.
* Avoid excessive gradients, neon colors, or decorative color effects unless they match the product style.
* Support dark mode when the project supports it.

## Components

* Prefer reusable and consistent UI components.
* Keep buttons, inputs, cards, dialogs, navigation, and other common elements visually consistent.
* Components should have clear visual states:

  * Default
  * Hover
  * Focus
  * Active
  * Disabled
  * Loading
  * Error
* Avoid creating multiple visually different versions of the same component without a clear reason.

## Interaction

* Make interactive elements visually identifiable.
* Provide clear feedback after user actions.
* Use appropriate hover, focus, active, and transition states.
* Keep animations subtle and purposeful.
* Avoid animations that distract from the task or reduce usability.
* Never rely on color alone to communicate important states.

## Forms

* Use clear labels and helpful placeholders.
* Make validation errors easy to understand and locate.
* Keep form layouts simple and predictable.
* Clearly distinguish required and optional fields.
* Provide loading and disabled states during submission.

## Responsive Design

* Design for different screen sizes instead of only scaling desktop layouts.
* Avoid fixed dimensions when flexible sizing is more appropriate.
* Ensure text, buttons, forms, and navigation remain usable on small screens.
* Handle long content, wrapping, and overflow gracefully.
* Test important layouts at mobile and desktop breakpoints.

## Accessibility

* Prefer semantic HTML elements.
* Ensure keyboard navigation works correctly.
* Provide visible focus states.
* Use accessible labels for controls.
* Maintain sufficient color contrast.
* Use ARIA only when semantic HTML is insufficient.
* Do not remove accessibility features for visual reasons.

## States

Always consider:

* Loading
* Empty
* Error
* Success
* Disabled
* Offline or unavailable states when relevant

Do not design only the ideal successful state.

## Visual Quality

Before considering UI work complete, check:

* Alignment
* Spacing
* Typography
* Color consistency
* Component consistency
* Responsive behavior
* Interactive states
* Accessibility
* Empty and error states

Fix obvious visual inconsistencies before finishing.

## Implementation Rules

* Inspect existing UI components and styles before creating new ones.
* Reuse existing design tokens and components whenever possible.
* Prefer small, targeted changes.
* Do not rewrite unrelated UI.
* Do not add dependencies for simple styling problems.
* Do not invent a design system when one already exists.
* Keep visual decisions consistent across the entire feature.
* If the project uses a UI library, follow its conventions instead of replacing it.
* If requirements are ambiguous, prefer the simplest design consistent with the existing application.

## Avoid

* Excessive rounded corners.
* Excessive shadows.
* Excessive gradients.
* Random colors.
* Inconsistent spacing.
* Too many font sizes.
* Tiny unreadable text.
* Unnecessary animations.
* Overly complex layouts.
* Decorative elements that reduce usability.
* UI patterns that look impressive but make the interface harder to use.
