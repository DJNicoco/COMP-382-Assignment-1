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

## Work/File Distribution

- **Nicole Zino**: Designed the DFA logic and implemented the TikZ diagram
  - `dfa_diagram.tex`
  - `Topic 4 DFA Diagram.pdf`
  - `README.md`
- **Inder Nijjar**: Set up the Beamer presentation and modified the position of the states
  - `dfa_diagram_modified.tex`
  - `DFA Modified Diagram.pdf`
  - `presentation.tex`

---

## Tools
- LaTeX
- TikZ
- Beamer

---

## Conclusion
In this project, we demonstrated how to create a correct 4-state DFA using LaTeX and TikZ. We also showed that the layout of the DFA can be easily modified without changing the underlying logic, as demonstrated by the modified diagram layout.

---

## References
Sipser, M. (2013). *Introduction to the Theory of Computation* (3rd ed.). Cengage Learning.

Overleaf. (n.d.). Online LaTeX editor. https://www.overleaf.com

AI tools were used for clarification, formatting assistance, and iterative refinement of explanations.
