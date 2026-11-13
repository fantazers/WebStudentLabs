[English](README.md) · [Русский](README.ru.md)

# JavaScript functions lab

Laboratory work for the Web Programming course: ten function exercises in vanilla JavaScript, checked by an automated Mocha suite.

## What it is

`core.js` holds ten function stubs with the task conditions in JSDoc comments. The solution fills in their bodies without changing function names, parameters, or the `module.exports` block. `core.spec.js` is the fixed test suite and is not edited.

## Structure

| File | Purpose |
| --- | --- |
| `core.js` | The ten functions to implement; the only file edited |
| `core.spec.js` | Mocha tests, 16 cases; must not be changed |
| `package.json` | Project metadata and the `npm test` command |
| `package-lock.json` | Pinned dependency tree for reproducible installs |

## Requirements

Node.js 18.18 or newer. Check the installed version with `node -v`.

## Install

```bash
npm install
```

## Tests

```bash
npm test
```

Expected result: `16 passing` and no `failing`. Before the solution all 16 tests fail; the number of passing tests grows as tasks are completed.

## Tasks

| # | Function | Requirement |
| --- | --- | --- |
| 1 | `isInteger(n)` | Check whether a number is an integer |
| 2 | `even()` | Return the array of even numbers from 2 to 20 |
| 3 | `sumTo(n)` | Sum 1 to n with a **loop** |
| 4 | `recSumTo(n)` | Sum 1 to n with **recursion** |
| 5 | `factorial(n)` | Factorial of n |
| 6 | `isBinary(n)` | Check whether a number is a power of two |
| 7 | `fibonacci(n)` | The n-th Fibonacci number |
| 8 | `getOperationFn(initialValue, operatorFn)` | A function that accumulates an operation result across calls |
| 9 | `sequence(start, step)` | Arithmetic progression generator |
| 10 | `deepEqual(a, b)` | Deep equality of two values |

Tasks 8 and 9 rely on closures: the returned function keeps its state between calls. Task 10 requires recursive traversal of object and array properties.

## Constraints

- Do not change function names, parameters, or the `module.exports` block in `core.js`.
- Do not change `core.spec.js`.
- Do not use third-party libraries.
- Use a loop in task 3 and recursion in task 4.
- The code must run in strict mode.

## Submission

1. Create a public GitHub repository and push this folder to it.
2. Add [@EdgarAbramian](https://github.com/EdgarAbramian) under **Settings → Collaborators → Add people**.
3. Attach the repository link to the submission.
