# Reasoning Test Set

This file contains the initial reasoning tasks for the Open LLM
Benchmark.

These tasks are intended to be used identically across evaluated
models.

## Evaluation Instructions

For each task:

1. Send the exact prompt to the model.
2. Record the complete response.
3. Do not modify the response before scoring.
4. Compare the answer with the expected answer or scoring rubric.
5. Record the result.
6. Record the model version and evaluation date.

---

## R001 — Ordering Constraints

### Difficulty
Easy

### Prompt

Five people — Alice, Bob, Carol, David, and Emma — are standing
in a line.

The following conditions apply:

- Alice is somewhere before Bob.
- Carol is immediately before David.
- Emma is not first.
- Bob is not last.

Which of the following could be a valid ordering?

A. Alice, Bob, Carol, David, Emma  
B. Bob, Alice, Carol, David, Emma  
C. Alice, Carol, David, Bob, Emma  
D. Emma, Alice, Carol, David, Bob

### Expected Answer

A

### Scoring

- `1` = A
- `0` = any other answer

---

## R002 — Numerical Reasoning

### Difficulty
Easy

### Prompt

A service processes 120 requests per minute.

Its processing capacity increases by 25%.

What is the new processing capacity per minute?

### Expected Answer

150 requests per minute.

### Scoring

- `1` = 150
- `0` = incorrect answer

---

## R003 — Multi-Step Reasoning

### Difficulty
Medium

### Prompt

A developer has 240 GB of available storage.

A model requires 80 GB.

The developer also needs three datasets requiring 20 GB,
15 GB, and 25 GB respectively.

After installing the model and all three datasets, how much
storage remains?

### Expected Answer

100 GB.

### Scoring

- `1` = 100 GB
- `0` = incorrect answer

---

## R004 — Constraint Reasoning

### Difficulty
Medium

### Prompt

A team must choose exactly two models from four models:

- Model A
- Model B
- Model C
- Model D

The following conditions apply:

- If Model A is selected, Model B cannot be selected.
- Model C can only be selected if Model B is selected.
- Model D cannot be selected together with Model C.

Which pair is valid?

A. A + B  
B. B + C  
C. C + D  
D. A + C

### Expected Answer

B

### Scoring

- `1` = B
- `0` = any other answer

---

## R005 — Information Analysis

### Difficulty
Hard

### Prompt

Three AI models were tested on the same task.

Model A completed 90 out of 100 tests.

Model B completed 84 out of 90 tests.

Model C completed 95 out of 120 tests.

Which model had the highest success rate?

### Expected Answer

Model B.

### Calculation

Model A:

90 / 100 = 90%

Model B:

84 / 90 ≈ 93.33%

Model C:

95 / 120 ≈ 79.17%

Therefore, Model B has the highest success rate.

### Scoring

- `1` = Model B
- `0` = any other answer

---

## Test Set Status

Version: 1.0

Number of tasks: 5

The tasks above are the initial public reasoning test set.

Future versions may add new tasks, but changes should be documented
so that results from different benchmark versions remain distinguishable.
