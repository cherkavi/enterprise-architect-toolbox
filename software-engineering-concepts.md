# Concepts

## Refactoring
*Refactoring (verb)* vs *Refactoring (noun)*

Refactoring is the process of clarifying and improving the internal structure of existing code without changing its external behavior.
* **As a verb:** To clean up code, remove technical debt, or optimize structure.
* **As a noun:** A specific, proven architectural change (e.g., "Extract Method" or "Move Field").

## Robustness Principle (Postel's Law)
**"Be conservative in what you do, be liberal in what you accept from others."**  
Deal with errors.  
Strict/isolated entity sending data over a boundary to a broader group.  
*Conservative* (on the sending side)  ----> *Liberal* (on the receiving side).  
**When sending data:** Your system should strictly follow specifications to ensure others can easily read your output.  
**When receiving data:** Your system should be accommodating, processing inputs gracefully even if they are slightly malformed or non-standard, as long as the meaning is clear.


## Error Handling Philosophy
* Expect errors and be able to react.  
* Software shouldn't just work under perfect conditions ("the happy path"); it must actively anticipate network drops, bad user input, and system failures. (*Defensive Programming* and *Fault Tolerance* )  
* Build robust recovery paths (like fallbacks or graceful degradation) so that an error in one component doesn't cause the entire system to crash.

## Conceptual Integrity
* **Core idea:**:
  *  Single
  *  coherent
  *  consistent design ideas.
* conceptual integrity means that a system's architecture should reflect a unified design philosophy. (Fred Brooks in *The Mythical Man-Month*)
* *Why it matters:* It is often better to have a system follow one consistent set of design decisions—even if a few choices are imperfect—than to have a patchwork of conflicting "good" ideas from different developers. It makes the system vastly easier to understand and maintain.

## Separation of Concerns (SoC)
* A clear boundary line separating **tech elem** (technical elements) from **funct elem** (functional elements).
* SoC is a design principle for separating a computer program into distinct sections, where each section addresses a separate concern or piece of logic.
* **Technical vs. Functional:** Keep infrastructure/technical logic (like database access, logging, or UI rendering) completely decoupled from functional business logic (the actual rules of how the application operates).
* **Information Hiding:** Modules should hide their inner workings behind clean interfaces, preventing external components from depending on their internal details.