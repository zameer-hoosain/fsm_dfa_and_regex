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

---

# DFA Example: Even binary numbers

---

# Some notation for the next few examples

Symbol:

Alternation:

Concatenation:

Repetition:

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
