# Coding Test Set

This file contains the initial coding tasks for the Open LLM
Benchmark.

The same prompts should be used for every evaluated model.

## Evaluation Instructions

For each task:

1. Send the exact prompt to the model.
2. Record the complete response.
3. Do not modify generated code before evaluation.
4. Run the code in the documented environment.
5. Record whether the required tests pass.
6. Record the model version and evaluation date.

---

## C001 — Python Function

### Difficulty
Easy

### Prompt

Write a Python function called `remove_duplicates` that accepts a
list of integers and returns a new list with duplicate values
removed while preserving the original order.

Example:

Input:
`[3, 1, 3, 2, 1, 5]`

Expected output:
`[3, 1, 2, 5]`

Do not modify the original input list.

### Evaluation

The solution must:

- Define `remove_duplicates`.
- Preserve the original order.
- Remove duplicate values.
- Return a new list.
- Not modify the input list.

### Scoring

- `1` = all requirements satisfied and tests pass
- `0` = otherwise

---

## C002 — JavaScript Bug Fix

### Difficulty
Medium

### Prompt

The following JavaScript function is intended to calculate the
sum of all numbers in an array:

```javascript
function calculateSum(numbers) {
    let total = 0;

    for (let i = 0; i <= numbers.length; i++) {
        total += numbers[i];
    }

    return total;
}
