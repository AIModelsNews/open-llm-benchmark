# Instruction-Following Test Set

This file contains the initial instruction-following tasks for the
Open LLM Benchmark.

The same prompts should be used for every evaluated model.

## Evaluation Instructions

For each task:

1. Send the exact prompt to the model.
2. Record the complete response.
3. Do not modify the response before scoring.
4. Check every required instruction.
5. Record the model version and evaluation date.

---

## I001 — Exact List Length

### Difficulty
Easy

### Prompt

List exactly five programming languages.

Requirements:

- Provide exactly five items.
- Use a numbered list.
- Do not include explanations.
- Do not include any additional text.

### Expected Structure

```text
1. Language
2. Language
3. Language
4. Language
5. Language
