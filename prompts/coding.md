# Coding Evaluation

## Purpose

This evaluation measures how effectively an AI model can solve
practical software-development tasks.

The goal is to evaluate coding ability using reproducible tasks
rather than relying only on general coding benchmark scores.

## Evaluation Rules

For comparable evaluations:

- Use the same task for each model.
- Record the exact model name and version.
- Record the programming language.
- Record the model configuration.
- Record the evaluation date.
- Do not modify the model's generated code before scoring.
- Record compilation and execution failures.
- Record whether tests pass.

## Test Categories

### 1. Code Generation

The model receives a programming requirement and must produce
working code.

Examples:

- Functions
- API endpoints
- Data processing
- Algorithms
- Utility scripts

### 2. Bug Fixing

The model receives code containing one or more bugs and must
identify and fix them.

### 3. Code Explanation

The model must explain existing code accurately and clearly.

### 4. Refactoring

The model must improve existing code while preserving its
required behavior.

### 5. Test Generation

The model must create tests for an existing implementation.

## Evaluation Criteria

Each coding task can be evaluated using:

| Metric | Description |
|---|---|
| Correctness | Does the solution produce the expected result? |
| Tests | Do the required tests pass? |
| Completeness | Were all requirements implemented? |
| Reliability | Does the solution work across test cases? |
| Code quality | Is the implementation understandable and maintainable? |
| Instruction following | Were the requested constraints respected? |

## Initial Test Set

The initial evaluation will contain manually reviewed coding
tasks.

Example structure:

| ID | Category | Language | Difficulty |
|---|---|---|---|
| C001 | Code generation | Python | Easy |
| C002 | Bug fixing | JavaScript | Medium |
| C003 | Refactoring | Python | Medium |
| C004 | API implementation | JavaScript | Hard |
| C005 | Test generation | Python | Hard |

These are task placeholders and are not benchmark results.

## Scoring

A coding task can receive:

- `1` = successful
- `0` = unsuccessful

A task is considered successful when the generated solution
satisfies the documented requirements and passes the required
tests.

For tasks requiring partial credit, a specific scoring rubric
will be documented.

## Execution Environment

When code execution is used, the benchmark should document:

- Operating system
- Programming language version
- Runtime version
- Dependencies
- Hardware
- Test framework

This information is necessary for reproducibility.

## Reliability

Important coding tasks should be evaluated multiple times when
the model configuration is non-deterministic.

The benchmark should record:

- Total runs
- Successful runs
- Failed runs
- Success rate

### Success Rate

```text
Success Rate = Successful Runs / Total Runs × 100
