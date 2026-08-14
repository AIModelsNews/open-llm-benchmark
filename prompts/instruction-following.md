# Instruction-Following Evaluation

## Purpose

This evaluation measures how accurately an AI model follows
explicit instructions and output constraints.

The goal is to measure whether a model can complete a task
without ignoring, changing, or adding requirements.

## Evaluation Rules

For comparable evaluations:

- Use identical prompts for each model.
- Record the exact model name and version.
- Record the model configuration.
- Record the evaluation date.
- Do not manually modify responses before scoring.
- Evaluate every required instruction.
- Record both successful and unsuccessful requirements.

## Test Categories

### 1. Format Compliance

The model must return information in a specified format.

Examples:

- JSON
- Markdown
- CSV
- Numbered lists
- Tables

### 2. Constraint Following

The prompt contains multiple requirements that must all be satisfied.

Examples:

- Word limits
- Required sections
- Forbidden terms
- Specific output structures
- Required number of items

### 3. Multi-Instruction Tasks

The model receives several instructions in a single prompt and
must satisfy them all.

### 4. Transformation Tasks

The model must transform provided information while preserving
specified requirements.

Examples:

- Summarization
- Reformatting
- Classification
- Translation
- Structured extraction

## Evaluation Criteria

| Metric | Description |
|---|---|
| Instruction compliance | Were all instructions followed? |
| Format compliance | Was the requested format respected? |
| Completeness | Were all required elements included? |
| Constraint compliance | Were restrictions respected? |
| Accuracy | Was the transformation correct? |
| Unwanted content | Did the response add information that was not requested? |

## Initial Test Set

The initial evaluation will contain manually reviewed tasks.

Example structure:

| ID | Category | Difficulty |
|---|---|---|
| I001 | Format compliance | Easy |
| I002 | Constraint following | Medium |
| I003 | Multi-instruction task | Medium |
| I004 | Structured extraction | Hard |
| I005 | Transformation | Hard |

These are placeholders and are not benchmark results.

## Scoring

A task can receive:

- `1` = all required instructions satisfied
- `0` = one or more critical instructions violated

For more detailed evaluations, partial scores may be used.

A documented scoring rubric should be provided whenever partial
credit is applied.

## Reliability

Important instruction-following tasks should be repeated when
the model configuration is non-deterministic.

Record:

- Number of runs
- Successful runs
- Failed runs
- Success rate

### Success Rate

```text
Success Rate = Successful Runs / Total Runs × 100
