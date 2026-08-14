# Reasoning Evaluation

## Purpose

This evaluation measures how reliably an AI model can solve
multi-step reasoning tasks and follow logical constraints.

The objective is to evaluate practical reasoning ability rather
than relying on a single public benchmark score.

## Evaluation Rules

For comparable model evaluations:

- Use the same prompts.
- Use the same task order when practical.
- Record the exact model version.
- Record sampling parameters.
- Record the evaluation date.
- Do not manually modify model responses before scoring.
- Record incorrect answers as failures.
- Record incomplete responses as failures when the task requires a complete solution.

## Test Categories

### 1. Logical Reasoning

Tests should require the model to identify relationships,
constraints, or logical conclusions.

### 2. Multi-Step Problems

Tests should require multiple connected steps before reaching
the final answer.

### 3. Constraint Following

Tests should include explicit constraints that must all be
satisfied.

### 4. Information Analysis

Tests should provide information that the model must analyze
before producing a conclusion.

## Initial Test Set

The initial benchmark will contain a small manually reviewed
test set.

Each test should have:

- A unique ID
- A prompt
- An expected answer or scoring criteria
- A difficulty level
- A category

Example:

| ID | Category | Difficulty |
|---|---|---|
| R001 | Logical reasoning | Easy |
| R002 | Logical reasoning | Medium |
| R003 | Multi-step reasoning | Medium |
| R004 | Constraint following | Hard |
| R005 | Information analysis | Hard |

## Scoring

Each response will be evaluated according to the requirements
of the individual task.

Possible scoring:

- `1` = successful
- `0` = unsuccessful

For tasks requiring partial credit, a documented scoring rubric
should be used.

## Reliability

Important reasoning tasks should be evaluated across multiple
runs when the model configuration is non-deterministic.

The benchmark should record:

- Number of runs
- Successful runs
- Failed runs
- Success rate

### Success Rate

```text
Success Rate = Successful Runs / Total Runs × 100
