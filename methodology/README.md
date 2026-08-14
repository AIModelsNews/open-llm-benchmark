# Benchmark Methodology

## Purpose

The Open LLM Benchmark evaluates AI models using practical tasks
representative of real-world developer and AI workloads.

The goal is not to produce a universal ranking of models, but to
provide transparent measurements that help users understand the
trade-offs between quality, reliability, speed, cost, and resource
requirements.

## Evaluation Principles

Each evaluation should follow these principles:

1. Use the same task set for comparable models.
2. Record the exact model version.
3. Document the hardware and software environment.
4. Keep prompts unchanged between comparable evaluations.
5. Run important tests multiple times when appropriate.
6. Record failures instead of excluding them.
7. Publish the evaluation date.
8. Clearly distinguish measured results from estimates.

## Evaluation Categories

### 1. Reasoning

Tests should evaluate the model's ability to:

- follow multi-step instructions
- solve logical problems
- analyze information
- explain its reasoning clearly

### 2. Coding

Coding evaluations may include:

- code generation
- debugging
- refactoring
- test generation
- code explanation

### 3. Instruction Following

Tests should evaluate whether the model:

- follows explicit requirements
- respects output constraints
- handles multiple instructions
- avoids adding unwanted information

### 4. Structured Output

Models may be tested on their ability to produce:

- JSON
- tables
- structured lists
- schema-compliant responses

### 5. Reliability

Important tasks should be repeated when possible.

Measurements may include:

- successful completions
- formatting failures
- incorrect answers
- tool-use failures
- consistency across runs

### 6. Speed

Depending on the inference environment, measurements may include:

- time to first token
- total response time
- tokens per second

Speed measurements should always include the hardware and software
environment used.

### 7. Memory Requirements

For locally evaluated models, record:

- system RAM
- GPU model
- VRAM
- model precision
- quantization
- context length

## Test Conditions

Every published evaluation should document:

- Model name
- Model version
- Quantization
- Hardware
- Operating system
- Inference framework
- Context length
- Sampling parameters
- Evaluation date

## Scoring

Scores should be calculated from the underlying measurements.

No model should receive a score simply because it is considered
popular or highly ranked elsewhere.

When an overall score is calculated, the weighting methodology will
be published alongside the results.

## Limitations

Benchmark results are dependent on:

- prompts
- datasets
- hardware
- software versions
- model versions
- sampling parameters
- evaluation methodology

Therefore, benchmark results should be interpreted as measurements
under specific conditions rather than permanent rankings.

## Reproducibility

Whenever possible, the project will publish:

- prompts
- datasets
- evaluation scripts
- configuration
- raw results

The objective is to allow independent developers and researchers to
reproduce or challenge the results.

## Changes to the Methodology

If the methodology changes substantially, the project will document
the change and identify which results were produced under the previous
methodology.
