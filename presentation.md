---
title: FSM, DFA and Regular Expressions
date: 2022-09-23
extensions:
  - image_ueberzug
styles:
  style: monokai
  table:
    column_spacing: 15
  margin:
    top: 2
    bottom: 0
  padding:
    top: 3
    bottom: 3
---

# Introduction

---

# Finite State Machines

- A Simple computational model
- State represents the entirety of what is needed for the system to work
- Finite number of states
- One start state
- States are connected using transitions
- May have one or more "accepting/terminating" states
  - Not a requirement for machines designed to run indefinitely

## Vending Machine Example:

![15](./fsm_example.gv.png)

---

# Why is this useful?

- String processing and matching
  - Compilers
- UIs
- E-commerce
- AI
- Video Games
- Control systems

---

# String processing with DFAs

- Deterministic Finite Automata (DFA) are simple Finite State Machines
- In a DFA a system can only exist in a single state at a time
- Each DFA has 5 essential properties:
  - `Q` - A finite set of all states
  - `Σ` - A finite set of all valid input symbols (the alphabet)
  - `δ: Q X Σ -> Q` - A transition function that goes from state to state given a symbol from the alphabet
  - `q₀ ∈ Q` A starting state (one of the states in `Q`)
  - `F ⊆ Q` A finite set of all accepting states (A subset of `Q`)
- For our purposes we will only explicitly note the states, starting state and final state. Assume that the alphabet is the entire ascii table unless otherwise specified.

---

# DFA Example: Even binary numbers

Consider a DFA with the following:

`Q` = [A, B, C]

`Σ` = 0, 1

`q₀` = A

`F` = [B]

Drawn as:
![15](./even_binary_dfa-1.gv.png)

Let's go through what happens when that DFM is fed an input of `1010`.

---

## **1**010

![25](./even_binary_dfa-2.gv.png)

---

## 1**0**10

![25](./even_binary_dfa-3.gv.png)

---

## 10**1**0

![25](./even_binary_dfa-4.gv.png)

---


## 101**0**

![25](./even_binary_dfa-5.gv.png)

---

# Some syntax for the next few examples

When showing the input that transition functions accept going forward, we can use the following
syntax to make things easier to read:

| Name          | Syntax             | Explanation                                    |
| ------------- | ------------------ | ---------------------------------------------- |
| Symbol        | a, b, c, 0, 1 etc. | Matches the exact character\*                  |
| Alternation   | a\|b               | Matches either a or b                          |
| Concatenation | ab                 | Matched exactly a followed by b                |
| Repetition    | a\*                | Matches the preceeding symbol 0 or more times. |

---

# DFA Example: Lex tokens

---

# DFA Example: Lex tokens cont.

---

# Why?

---

# Regex basics

Character classes

Range

. (dot)

Word, digit, and space classes

---

# Regex basics cont.

Escaping characters

Numeric quantifiers

## Seem familiar?

# DFA Example: Phone numbers

---
