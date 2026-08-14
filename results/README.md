# Benchmark Results

This directory contains the results of evaluations performed using
the Open LLM Benchmark methodology.

## Important

Results are only published after a model has been evaluated using
the documented test set and conditions.

No estimated, simulated, or invented scores are published.

## Result Format

Each evaluation should document:

- Model name
- Model version
- Evaluation date
- Hardware
- Software/inference framework
- Quantization or precision
- Sampling parameters
- Number of test runs
- Test set version

## Categories

Results will be organized by evaluation category:

- Reasoning
- Coding
- Instruction following

Additional categories may be added in future benchmark versions.

## Example Result Structure

| Model | Category | Tests | Successful | Score |
|---|---|---:|---:|---:|
| Example Model | Reasoning | 5 | — | Not evaluated |

The example above is a format demonstration only and is not a
real benchmark result.

## Reproducibility

Where possible, each published result should include enough
information for another developer to reproduce the evaluation.

This includes:

- Exact model identifier
- Model version
- Prompt set version
- Hardware
- Software
- Configuration
- Evaluation date
- Raw results

## Versioning

The benchmark test sets are versioned.

Results should identify the test-set version used during evaluation.

For example:

```text
Benchmark version: 1.0
Reasoning tests: 1.0
Coding tests: 1.0
Instruction-following tests: 1.0
