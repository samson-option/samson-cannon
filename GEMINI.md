# Samson Cannon - Project Context

## Project Overview

**Samson Cannon** is the creative and technical engine for "The Reset Order," a system designed to restore personal sovereignty and aid in addiction recovery. It focuses on building high-fidelity AI personas (Coach Bear, Dr. Love, Wingman) using a **Reference-Driven Design** philosophy.

Unlike traditional projects that start with broad vision documents, Samson Cannon grounds every feature and persona in specific, "gritty" truths and real-world exemplars (e.g., specific film characters, therapeutic models, biographies).

## Architecture & Directory Structure

The project is organized logically, moving from abstract philosophy to concrete implementation:

*   **`01_manifesto/`**: The "Why". Contains the foundational beliefs, mission, and culture of The Reset Order.
*   **`02_solution/`**: The "What". Defines the recovery framework, the platform strategy, and the roles of the AI coaches (Coach Bear, Dr. Love).
*   **`03_brand/`**: The "Vibe". Creative DNA, copywriting voices, and visual directives.
*   **`04_implementation/`**: The "How".
    *   **`how-we-build.md`**: The core engineering directive. Read this to understand the "Reference-Driven" philosophy.
    *   **`personas-pipeline/`**: Schemas and logic for compiling "Character Bibles" and "Reasoning Patterns" for the AI agents.
*   **`05_research/`**: The "Raw Material". Academic papers and articles on addiction, dopamine, and psychology that serve as the ground truth for the system.
*   **`.github/`**: Automation workflows, specifically for "Gemini" interactions (triage, review, invoke).

## Technical Setup

The project is primarily a Python-based system (requires Python >= 3.13), though much of the current value lies in the structured data and schemas.

### Prerequisites

*   Python 3.13+

### Building & Running

Currently, the codebase uses a simple entry point:

```bash
python main.py
```

*Note: The project uses `pyproject.toml` for dependency management.*

## Development Philosophy: Reference-Driven Design

**Crucial Mandate:** Do not rely on generic "vision" statements.
When contributing to this project, adhere to the 5-step process outlined in `04_implementation/how-we-build.md`:

1.  **Identify Exemplars:** Who/what are we modeling? (e.g., "Denis Villeneuve's lighting," "A specific military mentor").
2.  **Define Attributes:** What specific traits matter?
3.  **Codify:** Create schemas/data structures to represent these traits (found in `04_implementation/personas-pipeline/schemas`).
4.  **Acquire Knowledge:** Gather raw data (Step 4 "SWAT Operation")—this is stored in `05_research` or similar knowledge bases.
5.  **Design System:** Build the AI/Product behavior based *only* on the acquired knowledge.

## Key Schemas

The heart of the AI personality engine lies in the JSON schemas within `04_implementation/personas-pipeline/schemas/`:
*   `character_bible.schema.json`: Defines the master structure for a persona.
*   `persona_voice_dna_analysis.schema.json`: Defines how a persona speaks.
*   `reasoning_pattern_extractor.md`: Logic for deriving AI thought processes.
