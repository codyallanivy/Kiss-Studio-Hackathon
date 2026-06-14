# 5-Minute Demo Script

Use the prepared project `northwind-brew`. Do not create a new project during the recording. The goal is to show the full governed workflow quickly.

## Setup

Open these before recording:

1. `http://localhost:8765/builder`
2. `http://localhost:8765`
3. Teams governance mock, if you are using it

Confirm the Command Center shows:

- Active project: `northwind-brew`
- Model: `foundry:gpt-4o`
- Gallery assets visible in Creative Studio

## 0:00-0:25 - Open With The Problem

Say:

"Most AI builder demos show output. The problem is what happens around the output. Context gets scattered, projects borrow the wrong memory, and models spend tokens before the work is actually scoped. KISS Studio is my answer to that: a local-first builder where AI work stays grounded, governed, and auditable."

## 0:25-1:00 - Builder Studio Hook

Show Builder Studio.

Point at Plan, Build, Code, Test, Export.

Say:

"I start here because this is the beginner-friendly front door. A user can describe an idea, get a plan, edit visually, inspect components, change styles, move into code, and test the result. So at first glance, it looks like a visual website builder."

Pause, then point at the Reveal Command Center button.

"But the important part is underneath. This button reveals the command layer that keeps the build under control."

Click **Reveal Command Center**.

## 1:00-1:45 - Reveal The Operating Layer

Show Command Center.

Point at the Foundry model badge, project selector, and dashboard panels.

Say:

"This is the operating layer. The active project is Northwind Brew, a prepared coffee-brand landing page. Foundry is connected as the reasoning tier, but KISS controls what project memory the model can use, what scope rules apply, and what gets logged."

Then say the IQ line:

"The IQ story is simple: Foundry IQ grounds answers in project knowledge, Fabric IQ turns requests into scope decisions, and Work IQ makes the work visible through readiness, health, and verification signals."

## 1:45-2:30 - Live Action 1: Scoped Memory

Use the Assistant or Project Ops chat.

Prompt:

```text
What is this project about, and what is Tier 1 scope?
```

Say while it answers:

"I am not asking for a generic marketing answer. I want the system to read the active project's files and explain the current scope."

Point at citations.

Say:

"The important detail is the citations. The answer is grounded in Northwind Brew's own memory, not another project and not a random chat history."

Optional safety prompt, only if you have time:

```text
What do you know about Ember Tides or NPCs in this project?
```

Say:

"This is the safety check. If unrelated project memory appears here, the system is not safe enough. It should keep the active project isolated."

## 2:30-3:20 - Live Action 2: Scope Gate

Go to Scope Gate.

Prompt:

```text
Add ecommerce checkout, loyalty rewards, and local delivery tracking.
```

Say:

"This is where the system behaves differently from a normal AI builder. A normal assistant might start building all of this. KISS checks the project vision first."

Point at verdict and tier.

Say:

"For Northwind Brew, Tier 1 is only the landing page, signup action, and foundation assets. Ecommerce, rewards, and delivery tracking sound useful, but they are not this sprint. The system warns or blocks and parks the request instead of spending time and tokens on the wrong work."

## 3:20-4:10 - Live Action 3: Creative Studio Assets

Go to Creative Studio.

Show the vision board and asset gallery.

Say:

"Now the same governance loop applies to creative work. This project already has a logo mark, hero composition, mobile signup mockup, palette card, and product card. These are not just decoration; they are foundation assets grounded in the project brief."

Click add asset if you want one live action.

Prompt:

```text
logo: warm neighborhood coffee brand mark for a beginner-friendly landing page
```

Say:

"Before creating an asset, the system searches the project references. If Foundry is on, it can use the model for a better SVG direction. If cloud tokens are off, the offline path still keeps the demo reliable."

## 4:10-4:35 - Optional M365 Governance Payoff

Show the Teams or M365 governance mock.

Say:

"This is the manager-facing payoff. The mock is not pretending to be live tenant data. It is a demo surface built from reasoning outputs and synthetic work signals, so a manager can see what was blocked, why, and where verification debt is building."

## 4:35-5:00 - Close

Say:

"KISS Studio turns AI output into governed project work. The visual builder helps beginners start. The Command Center keeps memory, scope, decisions, verification, assets, and model choice under control. That is the thesis behind DigitalQuill Labs: help people build with AI without losing context, scope, or ownership."

## Backup Prompts

Use these if a live step fails:

```text
What is this project about, and what is Tier 1 scope?
```

```text
Add ecommerce checkout, loyalty rewards, and local delivery tracking.
```

```text
Summarize this project's blockers and next best work.
```

```text
logo: warm neighborhood coffee brand mark for a beginner-friendly landing page
```

## What Not To Do

- Do not create a new project live.
- Do not explain every panel.
- Do not mention the old fantasy template unless asked.
- Do not spend time debugging asset generation on camera.
- Do not say "the AI refused." Say "the system governed the request."

