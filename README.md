# Assignment 1 – DFA State Diagram using TikZ and Beamer

## Project Overview
In this project, we demonstrate how to draw a 4-state Deterministic Finite Automaton (DFA) using LaTeX with the TikZ package on a single PDF page.  
The DFA follows the standard state-diagram notation presented in the course textbook and lecture slides.  
We also demonstrate how the position of states can be easily adjusted by modifying the TikZ code, highlighting the flexibility of programmatic diagram generation.

---

## DFA Description
The DFA consists of four states: {q0, q1, q2, q3}, over the alphabet {0,1,2,3}.

Each state qi represents the remainder i (mod 4) of the sum of input symbols read so far.
The start state q0 represents a sum congruent to 0 modulo 4.
State q3 is the accepting state and represents a sum congruent to 3 modulo 4.

For each input symbol d ∈ {0,1,2,3}, the transition function moves from state qi to state q((i + d) mod 4).
This ensures that all transitions are deterministic and that the DFA correctly tracks the running sum modulo 4.

---

## Work Distribution

- **Nicole Zino**: Designed the DFA logic and implemented the TikZ diagram  
- **Inder Nijjar**: Set up the Beamer presentation and handled layout adjustments

---

## Tools
- LaTeX
- TikZ (automata and positioning libraries)
- Beamer

---

## References
Sipser, M. (2013). *Introduction to the Theory of Computation* (3rd ed.). Cengage Learning.

AI tools were used for clarification, formatting assistance, and iterative refinement of explanations.
