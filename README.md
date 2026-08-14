# Open LLM Benchmark

An open and reproducible benchmark for comparing AI models across
real-world developer and AI workloads.

🌐 **Website:** [AIModelsNews](https://aimodelsnews.com/)

## 🎯 About

The goal of this project is to evaluate AI models using practical
tasks rather than relying exclusively on public leaderboard scores.

The benchmark is designed to measure several dimensions of model
performance and deployment suitability.

## 📊 Evaluation Areas

The benchmark will evaluate models across:

- Reasoning
- Coding
- Instruction following
- Structured output
- Context handling
- Response speed
- Reliability
- Memory requirements
- Hardware requirements
- Cost

## 🤖 Models

Models will be added progressively as evaluations are completed.

Planned categories include:

- Open-weight large language models
- Small language models
- Coding models
- Reasoning models
- Multimodal models

Model results will only be published after the corresponding
evaluation has been performed.

## 🧪 Methodology

Each model evaluation should document:

1. Model name and version
2. Model size when available
3. Quantization or precision
4. Hardware configuration
5. Software/inference framework
6. Prompt or test dataset
7. Number of evaluation runs
8. Evaluation metrics
9. Measurement conditions
10. Date of evaluation

The objective is to make results as reproducible as possible.

## 📈 Metrics

Depending on the task, measurements may include:

| Metric | Description |
|---|---|
| Quality | Overall task performance |
| Accuracy | Correctness of the result |
| Reliability | Consistency across repeated runs |
| Latency | Response time |
| Throughput | Tokens processed per second |
| Memory | RAM/VRAM requirements |
| Cost | Estimated inference cost |
| Format compliance | Ability to follow required output formats |

Not every metric applies to every model or task.

## 🔬 Reproducibility

Benchmark results should include enough information for another
developer to understand how the evaluation was performed.

When possible, the project will publish:

- Test prompts
- Evaluation datasets
- Scripts
- Configuration files
- Raw measurements
- Aggregated results

Results may change as models, software, and hardware evolve.
Every published result should therefore include an evaluation date.

## 📋 Results

No benchmark results are published yet.

Results will be added after real evaluations are completed.

Example structure:

| Model | Reasoning | Coding | Speed | Reliability | VRAM |
|---|---:|---:|---:|---:|---:|
| Coming soon | — | — | — | — | — |

**Important:** Placeholder values are not benchmark results.

## 🗂️ Project Structure

The repository will gradually contain:

```text
open-llm-benchmark/
├── README.md
├── methodology/
├── prompts/
├── evaluations/
├── results/
├── scripts/
└── datasets/
