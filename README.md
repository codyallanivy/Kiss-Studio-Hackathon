# KISS Studio - Agents League Submission

KISS Studio is a local-first command center for AI-assisted builders. It combines a beginner-friendly Builder Studio with a project memory and governance layer that keeps AI work scoped, cited, and tied to real project value.

The project was built for Microsoft Agents League @ AISF 2026. The contest requires integration with at least one Microsoft IQ intelligence layer; KISS Studio demonstrates a Foundry IQ-style scoped retrieval layer, Fabric IQ-style semantic rules, and Work IQ-style capacity signals.

## Problem

AI builders can generate a lot of output, but output is not the same as progress. Common failure modes are:

- Losing project context between AI sessions
- Mixing memory from unrelated projects
- Spending tokens on out-of-scope work
- Generating assets without checking the actual project need
- Leaving decisions, risk, and verification scattered across chats

KISS Studio turns those concerns into an operating layer around agentic building.

## What It Does

- Command Center: switch projects, choose model tier, inspect project health, ask scoped questions, and run scope gates.
- Builder Studio: visual Plan -> Build -> Code -> Test workflow for beginner-friendly app/site creation.
- Creative Studio: survey intake that turns an idea into a governed project, creation document, and gallery assets.
- Scoped IQ retrieval: active project files are used first; shared KISS method docs are process support; other project memory is excluded by default.
- Foundry-enhanced assets: gallery generation searches project references before creating assets. With Foundry active it can generate stronger SVG assets; with an Azure image deployment it can generate PNG concept assets.
- Model ladder: Microsoft Foundry/Azure when configured, local Ollama when available, deterministic offline fallback otherwise.

## Microsoft IQ Integration

KISS Studio uses three IQ-inspired layers:

- Foundry IQ: local grounded retrieval with citations and strict project boundaries before prompts are sent to Foundry.
- Fabric IQ: semantic policy/rule checks for scope tiers, readiness, and governance.
- Work IQ: synthetic work-signal data for capacity-aware recommendations and team readiness.

The important design choice is that Foundry is the reasoning/model tier, but KISS Studio controls what memory Foundry is allowed to see.

## Demo Flow

Recommended 5-minute recording:

1. Open Builder Studio and show the visual builder hook.
2. Click **Reveal Command Center** and show the real control layer.
3. Use the prepared `northwind-brew` project.
4. Ask a project-scoped question and show citations.
5. Run a scope gate and show Tier/WARN/BLOCK governance.
6. Show the Creative Studio vision board and foundation asset gallery.

See `DEMO_SCRIPT.md` for a timed script.

## Prepared Demo Project

`demo-project/northwind-brew` is the recommended recording project. It is a polished neighborhood coffee brand landing-page example with:

- Scoped KISS memory files
- Tier 1 launch-page scope
- A useful board, health state, and decision log
- A vision board
- Starter foundation assets for the gallery

Use it for the recorded demo instead of creating a new project live.

## Quick Start

Requirements:

- Python 3.11+
- Optional: Ollama for local models
- Optional: Azure OpenAI / Microsoft Foundry credentials for cloud model and image generation

Run:

```powershell
start.bat
```

Then choose:

- `1` for Command Center
- `2` for the Track 2 reasoning demo
- `3` for Builder Studio
- `4` for Teams governance mock

The main dashboard runs at:

```text
http://localhost:8765
```

Builder Studio runs at:

```text
http://localhost:8765/builder
```

## Azure / Foundry Setup

Copy `foundry-track2/.env.example` to `foundry-track2/.env` and configure:

```text
AZURE_OPENAI_ENDPOINT=
AZURE_OPENAI_KEY=
AZURE_AI_MODEL_DEPLOYMENT=gpt-4o
AZURE_AI_IMAGE_DEPLOYMENT=
AZURE_OPENAI_IMAGE_API_VERSION=2025-04-01-preview
```

If `AZURE_AI_IMAGE_DEPLOYMENT` is empty, gallery assets still improve through Foundry-generated SVG when the Foundry chat model is active. If an Azure image deployment such as `gpt-image-*` is configured, the gallery can produce PNG assets.

## Safety Notes

- Do not commit `.env` or keys.
- Project memory is scoped by active project.
- Fantasy/demo templates are not part of the submission path.
- Generated traces and local verification artifacts are ignored.

## Thesis Origin

This project comes from the DigitalQuill Labs thesis: AI should create value, not just output. The product is not anti-AI; it is anti-waste. It keeps goals, context, decisions, risk, and compute usage visible so builders can keep the human client in control.
