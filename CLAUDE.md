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

### 01_manifesto/ - The WHY (Foundational Beliefs)

Core documents defining the organization's irreducible beliefs and identity:

- `axioms.md` - The six foundational axioms upon which everything is built
- `mission.md` - What we do, who we serve, how we differ
- `values.md` - Operating principles (non-negotiable)
- `origin.md` - The founder's story and the gap that created us
- `culture.md` - The Phalanx model and three theaters of connection

### 02_solution/ - The WHAT (Recovery Framework)

The methodology and platform strategy:

- `framework.md` - Complete 9-month recovery methodology (Scan-Engage-Secure-Reload loop)
- `philosophy.md` - Theoretical foundations (why existing solutions fail, primacy of motivation)
- `knowledge-base.md` - Recovery Bible with indexed knowledge blocks
- `platform/personas.md` - AI persona definitions (Coach Bear, Dr. Love, Wingman)
- `people/founder.md` - Founder profile

### 03_brand/ - The VIBE (Creative Expression)

Brand voice and visual direction:

- `voice.md` - Brand voice principles and persona voice summaries
- `visual/emotional-scene-directive.md` - Scene generation canon (15 emotional journey stages)
- `copywriting/` - Voice DNA JSON extracts for personas

### 04_implementation/ - The HOW (Engineering)

Technical specifications and build processes:

- `how-we-build.md` - Core engineering philosophy (Reference-Driven Design)
- `mvp-jobs.md` - MVP feature specification
- `metrics-framework.md` - Dopamine Resilience Score and 9-month KPI tracking
- `onboarding-ux.md` - User profile schema and onboarding flow
- `personas-pipeline/` - Schemas and compilers for persona generation

### 05_research/ - Ground Truth

Academic papers on addiction, dopamine, psychology sourced from Gabor Mate, Anna Lembke, James Clear, and others.

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

## Core Concepts

Key terminology used throughout the canon:

- **Sovereignty**: Executive agency over one's own mind and life (the end goal)
- **Dopamine Fitness**: Measure of reward system regulation and resilience
- **The Phalanx**: Tactical brotherhood model for mutual accountability
- **The Loop**: Scan-Engage-Secure-Reload daily practice cycle
- **Three Domains**: Neurochemical reset, behavioral reconditioning, identity reconstruction

## GitHub Automation

Gemini CLI workflows in `.github/workflows/` handle issue triage and code review.
