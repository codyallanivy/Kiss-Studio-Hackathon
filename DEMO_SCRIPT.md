# 5-Minute Demo Script

## 0:00-0:25 - Problem

"AI builders are powerful, but most workflows still lose context between sessions, mix project memory, and spend tokens creating output that may not move the project forward. KISS Studio is a local-first command center for AI-assisted building."

"This came from my DigitalQuill Labs thesis: I am not anti-AI; I am anti-waste. The goal is to help builders keep durable context, clear decisions, and intentional compute use."

## 0:25-1:00 - Builder Studio Hook

Open Builder Studio.

"At first this looks like another AI website builder. You can plan, build, inspect components, edit styles, and move toward code and testing."

Show the build space briefly.

"But the real differentiator is not just the canvas. It is the command layer underneath."

Go back to Command Center.

## 1:00-1:50 - Command Center Reveal

Show the project selector, model selector, and Foundry badge.

"Each project has its own memory and files. When I switch projects, the system should not retrieve another project's context. Foundry is the reasoning layer, but KISS controls what memory Foundry is allowed to see."

## 1:50-2:35 - Scoped Memory Demo

Select `northwind-brew`.

Ask:

```text
What is this project about, and what is Tier 1 scope?
```

Point to citations from `northwind-brew`.

Switch to `pizza-shop`.

Ask:

```text
What do you know about Ember Tides, NPCs, or the Drowned Shrine in this project?
```

Expected point:

"It refuses to pull fantasy memory into the active project. This is reliability and safety at the retrieval layer."

## 2:35-3:25 - Reference-Grounded Gallery Asset

Go to Creative Studio or gallery.

Add an asset:

```text
logo
warm neighborhood coffee brand mark for a beginner-friendly landing page
```

Point out:

- Reference search runs before generation
- The result includes citations
- Mode is `foundry-svg` or `foundry-image` if Azure image deployment is configured
- Offline fallback still works

## 3:25-4:15 - Scope Gate

Use the scope gate:

```text
Add delivery tracking, analytics dashboard, and a customer rewards app.
```

Expected point:

"Instead of just building everything, KISS classifies scope, parks Tier 2/3 work, and protects the sprint."

## 4:15-4:45 - Model Ladder

Show the model selector:

- Foundry for strongest reasoning
- Ollama for local/private/cheaper use
- Offline for deterministic fallback

"This makes the workflow usable even when cloud tokens are off, while Foundry enhances reasoning and asset generation when available."

## 4:45-5:00 - Close

"Most AI coding demos show output. KISS Studio shows the operating system around output: memory, scope, decisions, verification, assets, and model choice. It is a builder for people who want ideas finished, not scattered across forgotten chats."

