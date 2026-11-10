# 🍳 senpai-cook-this

### Your code is the ingredient. Senpai is the chef. Slop is NOT on the menu.

A Claude Code skill that implements your requirements, keeps your codebase clean, and does one thing most developers conveniently forget:

**DOCUMENT THE DAMN THING.**

## 🚀 Installation & Usage

### 1. Add the marketplace

Open Claude Code and run:

```bash
/plugin marketplace add sagarkpro/sagar-senpai-marketplace
```

### 2. Install Senpai Skills

```bash
/plugin install senpai-skills@sagar-senpai-marketplace
```

### 3. Reload plugins

```bash
/reload-plugins
```

### 4. Let Senpai cook 🍳

Use the skill with your requirements:

```text
/senpai-skills:senpai-cook-this [REST OF THE PROMPT HERE]
```

**Example:**

```text
/senpai-skills:senpai-cook-this Implement a new booking
cancellation API with proper validation and documentation.
```

That's it. Three commands and you're ready to cook.

---

## 🐧 Meet Senpai

```text
                    ／＞　 フ
                   | 　_　_| 
                 ／` ミ＿xノ
                /　　　　 |
               /　 ヽ　　 ﾉ
              │　　|　|　|
          ／￣|　　 |　|　|
          | (￣ヽ＿_ヽ_)__)
          ＼二つ

       ╔══════════════════════════════════╗
       ║  ARCH LINUX  ::  SENPAI TERMINAL ║
       ╠══════════════════════════════════╣
       ║                                  ║
       ║  $ senpai --cook                 ║
       ║                                  ║
       ║  [✓] Requirements understood     ║
       ║  [✓] Business logic respected    ║
       ║  [✓] Clean code prepared         ║
       ║  [✓] Documentation updated       ║
       ║  [✗] Unnecessary abstractions    ║
       ║  [✗] Hallucinated API fallbacks  ║
       ║  [✗] Code slop detected          ║
       ║                                  ║
       ║  STATUS: COOKING...              ║
       ╚══════════════════════════════════╝

            (ง •̀_•́)ง  🍳
          "Omae wa mou refactor shindeiru."
```

## 🧑‍🍳 What does Senpai do?

You give it a feature. It cooks it.

But unlike your average AI coding assistant, Senpai doesn't just throw 47 files at the wall and call it a day.

It follows a few ground rules:

- Implements what you actually asked for.
- Keeps business logic where it belongs.
- Prefers readable code over clever code.
- Doesn't invent data to make the UI look pretty.
- Doesn't introduce unnecessary fallbacks.
- Maintains documentation at THREE levels.
- Leaves Git operations to the human chef.

Basically, **less AI magic, more engineering discipline.**

## 📚 The Holy Trinity of Documentation

Every feature deserves documentation. Not just a random README that nobody reads.

| Layer | Audience | Purpose |
|---|---|---|
| Developer Docs (`.md`) | Developers | Features, business context, WHY, architecture and impact analysis |
| Machine Docs (`.md`) | AI / Coding Agents | Deep file references, implementation details and technical workflows |
| User Guide (`.html`) | End Users | Beautiful, minimal documentation with practical examples |

### Modifying existing features?

Don't just change the code and disappear.

Update all three documentation layers, including a changelog explaining:

- What existed before.
- What changed.
- Why it changed.

Each document maintains its own versioning.

**Documentation is part of the feature. Not an optional side quest.**

## 📏 The Kitchen Rules

### 1. Keep the code readable

- No unnecessarily fancy syntax.
- Maximum one ternary per statement.
- Maximum two chained LINQ methods.
- Avoid deeply nested conditions.
- Prefer explicit `if-else` statements.
- Use intermediate variables.
- Prefer readable code over compressed one-liners.

If someone needs three coffees to understand your one-liner, it's probably not a good one-liner.

### 2. UI is not your business analyst

The UI has TWO jobs:

- Display data.
- Collect user input.

That's it.

No business calculations. No inventing values. No interpreting business rules.

If the UI needs to calculate a booking total, the API should provide that total.

Basic presentation transformations, such as formatting dates, are perfectly fine.

If a requirement demands business logic in the UI, flag it to the user instead of silently implementing it.

**The UI is a waiter, not the chef.**

### 3. Stop making things up

Missing API data?

- Missing role? Show an empty value.
- Missing price? Don't invent one.
- Missing field? Flag it.
- Missing business requirement? Ask.

No fake defaults. No substitute values. No imaginary data.

### 4. Component discipline

- Components should stay below 250 lines.
- Avoid tiny components below 100 lines unless reusable or distinctly useful.
- No spread operators.
- Maximum one optional chaining operator per expression.
- Keep related UI logic together.

### 5. Comments are not novels

Comments should explain WHY, not WHAT.

One or two lines are usually enough.

Your code should explain itself. If it needs a documentary narrator, something is wrong.

### 6. Git belongs to the human

No commits. No pushes. No merges. No rebases.

Unless explicitly instructed.

Senpai cooks. The human decides when dinner gets served.

## 🎯 The Philosophy

We don't optimize for:

- Fewest lines of code.
- Most sophisticated syntax.
- Maximum abstraction.
- Impressing other developers with unnecessary complexity.

We optimize for:

**Code that another developer can understand, review, modify, and maintain without questioning their career choices.**

---

## ⚠️ Final Warning

Senpai has zero tolerance for:

- Business logic disguised as UI code.
- Unnecessary fallbacks.
- Overengineered solutions.
- Documentation left to rot.
- Clever code that nobody understands.

> Anyone can generate code.  
> Not everyone can engineer software.

---

<sub>Powered by Claude Code. Made with 🍳, Linux energy, engineering discipline, and an unreasonable hatred for code slop.</sub>

**senpai-cook-this — Don't just write code. Cook it properly.**