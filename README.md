# Pseudocode Learning

A structured, language-independent reference for fundamental programming concepts and introductory algorithms expressed in pseudocode.

## Overview

This repository contains 11 topic-focused documents organized from basic program structure to conditions, loops, arrays, and algorithms.

Each document introduces a concept and demonstrates it through practical examples of increasing complexity. The notation focuses on program logic rather than the syntax of a specific programming language.

The planned learning scope is complete. The repository is maintained as a reference for designing algorithms, reviewing programming fundamentals, and translating logic into source code.

## Contents

| Section | Documents | Coverage |
|---|---|---|
| **01 — Basics** | [Variables](01-basics/variables.md) · [Input and output](01-basics/input-output.txt) · [Operators](01-basics/operators.txt) | Assignment, reassignment, data values, user input, output, arithmetic, `MOD`, and `DIV` |
| **02 — Conditions** | [Conditions and logical operators](02-conditions/nested-conditions.md) · [IF / ELSE](02-conditions/if-else.md) · [SWITCH / CASE](02-conditions/switch-case.md) | Comparisons, boolean logic, ranges, nested decisions, authentication checks, menus, and multi-case selection |
| **03 — Loops** | [FOR loops](03-loops/for-loop.md) · [WHILE loops](03-loops/while-loop.md) | Counting, stepping, accumulation, validation, nested loops, list traversal, and repetition based on conditions |
| **04 — Arrays** | [Array examples](04-arrays/array-examples.md) | Indexing, mutation, length, traversal, aggregation, searching, reversing, user input, and nested arrays |
| **05 — Algorithms** | [Factorial](05-algorithms/factorial.md) · [Prime numbers](05-algorithms/prime-number.md) | Iterative and recursive factorials, prime validation, prime enumeration, and optimized divisor checks |

## Pseudocode Conventions

| Construct | Notation | Purpose |
|---|---|---|
| Program boundaries | `START` / `END` | Define the beginning and end of a program |
| Assignment | `SET name TO value` | Store or update a value |
| Input | `INPUT name` | Read a value |
| Output | `PRINT value` | Display a value |
| Conditional branch | `IF` / `ELSE IF` / `ELSE` | Select a path based on conditions |
| Multi-case selection | `SWITCH` / `CASE` / `DEFAULT` | Match one value against multiple options |
| Count-controlled loop | `FOR` / `END FOR` | Repeat over a range or collection |
| Condition-controlled loop | `WHILE` / `END WHILE` | Repeat while a condition remains true |
| Function | `FUNCTION` / `RETURN` | Define reusable logic and return a result |
| Array operations | `ADD`, `REMOVE`, `LENGTH` | Modify or inspect a collection |
| Numeric operations | `MOD`, `DIV`, `SQRT` | Perform remainder, integer division, and square-root operations |

Keywords are written in uppercase, and indentation represents nested control-flow blocks.

## Example

```text
START
  SET numbers TO [10, 25, 7, 42, 18]
  SET largest TO numbers[0]

  FOR each number IN numbers
    IF number > largest THEN
      SET largest TO number
    END IF
  END FOR

  PRINT "Largest number: " + largest
END
```

The same algorithm can be translated into Python, Java, C#, JavaScript, or another programming language without changing its underlying logic.

## Usage

The material is ordered by topic and can be followed sequentially:

1. Start with variables, input, output, and operators.
2. Continue with conditional logic and selection.
3. Study count-controlled and condition-controlled loops.
4. Apply those concepts to arrays and collections.
5. Review the factorial and prime-number algorithms.

The repository can also be cloned locally:

```bash
git clone https://github.com/ErkanSoftwareDeveloper/pseudocode-learning.git
cd pseudocode-learning
```

No installation, runtime, or external dependencies are required.

## Scope

Pseudocode has no universal syntax. The notation used here intentionally prioritizes readability and consistency over language-specific rules.

The examples are designed to describe program behaviour and algorithmic flow. They are documentation and are not intended to be executed directly.
