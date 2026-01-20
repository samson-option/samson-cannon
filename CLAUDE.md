# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Samson Cannon is the creative and technical engine for "The Reset Order" - a system for addiction recovery that builds high-fidelity AI personas (Coach Bear, Dr. Love, Wingman) using Reference-Driven Design philosophy.

## Commands

```bash
# Run the application
python main.py
```

Python 3.13+ required. Uses `pyproject.toml` for dependency management.

## Architecture

The repository is organized from abstract philosophy to concrete implementation:

- **`01_manifesto/`** - Foundational beliefs, mission, and culture (the "Why")
- **`02_solution/`** - Recovery framework, platform strategy, AI coach definitions (the "What")
- **`03_brand/`** - Creative DNA, copywriting voices, visual directives (the "Vibe")
- **`04_implementation/`** - Engineering directives and persona pipelines (the "How")
  - `how-we-build.md` - Core engineering philosophy (Reference-Driven Design)
  - `personas-pipeline/schemas/` - JSON schemas for Character Bibles and Reasoning Patterns
- **`05_research/`** - Academic papers on addiction, dopamine, psychology (ground truth)

## Development Philosophy: Reference-Driven Design

**Critical:** Do not rely on generic "vision" statements. Follow the 5-step process in `04_implementation/how-we-build.md`:

1. **Identify Exemplars** - Find concrete references to model (people, products, characters)
2. **Define Attributes** - List specific traits and why they matter
3. **Codify** - Create schemas/data structures in `04_implementation/personas-pipeline/schemas/`
4. **Acquire Knowledge** - Gather raw data ("SWAT Operation") into `05_research/` or knowledge bases
5. **Design System** - Build AI/product behavior based only on acquired knowledge

## Key Schemas

Persona definitions live in `04_implementation/personas-pipeline/schemas/`:
- `character_bible.schema.json` - Master structure for a persona
- `persona_voice_dna_analysis.schema.json` - How a persona speaks
- `persona_reasoning_patterns_and_heuristics_*.schema.json` - AI thought processes

## GitHub Automation

Gemini CLI workflows in `.github/workflows/` handle issue triage and code review.
