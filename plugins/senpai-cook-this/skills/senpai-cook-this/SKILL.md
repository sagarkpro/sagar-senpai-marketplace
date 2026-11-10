---
name: senpai-cook-this
description: Implement user requirements with simple, readable code rules and maintain 3-level docs (developer md, machine md, end-user html) with changelogs in /docs.
---

Implement the user's requirements, then do one extra step: maintain docs at 3 levels.

## Docs

1. **Developer doc (md):** features, business side, WHY it's done, high-level technical details. Include a detailed reference-by-section for impact analysis when modifying a feature.
2. **Machine doc (md):** deep file references, what's done, how it works, why. Code-heavy.
3. **End-user guide (html):** examples, beautiful, minimal.

Modifying an existing feature: update the existing docs and add a changelog to all 3 (what it was before, what changed, why). Choose versioning per doc yourself.
Ask the user questions (why, business side) when it improves doc accuracy and reduces slop. Docs should generally live in repo’s /docs folder unless explicitly mentioned.

## Generic Coding Rules (UI + API)

- No fancy/complex syntax. No inline comparisons that execute methods (e.g. `bookingStrategy == "bookandpay" && BookAsync()`); use simple if-else.
- Max one ternary per statement; use if-else for complex conditions.
- Max two chained LINQ methods; split complex queries into steps.
- Avoid deep nesting and complex one-liners; use intermediate variables and explicit statements.
- Prefer simple loops over complex LINQ when more readable.
- Comments: 1-2 lines, explain why, not the obvious. Avoid long, multi-line comments.
- Keep code simple, readable, maintainable. More readable lines beat fewer complicated lines (easy to review and maintain).

## UI Rules

- Components <250 lines; split if larger. Don't make tiny components (<100 lines) unless reusable or distinct; keep closely related UI logic together.
- No spread operator (`...`); assign properties explicitly.
- Max one optional chaining operator per expression (no `booking?.payment?.status`); use intermediate variables or null checks.
- No business logic or business calculations in UI (e.g. total = base + taxes); the API handles them. UI consumes final values.
- If a requirement needs business logic or non-presentational data transformation, flag it to the user; don't implement it.
- Allowed: basic type/presentation transforms (e.g. raw date to readable date).
- No fallbacks or substitute values for missing API data. Show API data as-is (missing role = empty, not `Client User`).
- Never assume, infer, or fabricate missing data; if the API doesn't provide a needed value, flag it.
- Principle: UI displays and collects data; it doesn't generate, calculate, or interpret business data.

## Git

- No Git operations (commit, push, merge, rebase, etc.) unless explicitly instructed; user normally does them.
- If instructed, state the potential impact first, especially for destructive/irreversible operations.