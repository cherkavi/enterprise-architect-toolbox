# 🏹 ArchiMate Relationships & Arrows Cheat Sheet

> **Purpose:** A practical guide to interpreting ArchiMate arrows to model relationships between enterprise architecture elements (Subjects, Objects, Structure, and Actions).

---
## 1. Core Syntax: Subject → Action → Object
aligns with [archimate aspects](./architecture-togaf-cheat-sheet.md#aspects)

*   **Subject (The Actor):** Represents the **Owner**, **Keeper**, or **Holder** of the action.
*   **Action:** The verb performing the operation.
*   **Object (The Target):** Represents the **Structure** that receives the action or outcome.

**Directionality:** 
* The **Tail** (start of arrow) represents the **Power Keeper** or the entity that initiates or holds the dependency. 
* The **Head** (end of arrow) represents the **Being Helped** or the structural target.

---
## 2. ArchiMate Relationship Categories

### A. Structural Relationships (The "What"), Tail 
Defines the static structure, composition, and responsibility of elements in the architecture.

| Notation Visual | ArchiMate       | Meaning & Context                                                                                                  |
| :---:           | :---            | :---                                                                                                               |
| `◇─`            | **Aggregation** | An element is composed of other parts, but parts can exist independently.                                          |
| `◆─`            | **Composition** | Indicates a whole-part relationship where parts are tightly bound.                                                 |
| `●─`            | **Assignment**  | Represents the allocation of responsibility (e.g., a Business Actor assigned to a Role). Responsible for doing job |

### B. Dependency Relationships (The "How" & "Access"), Head
Defines how elements rely on each other to achieve objectives. This is the most heavily used section in practical mapping.

| Notation Visual     | ArchiMate Standard Equivalent         | Meaning & Context                                                                                             |
| :---:               | :---                                  | :---                                                                                                          |
| `─>` (Solid)        | **Serving** / **Used by**             | A solid line showing "Power Keeper" (`Tail`) is being used to help the target (`Head`).                       |
| `<--->` (Dashed)    | **Access**  read or write             | Represents read (r) or write (w) access to data or physical objects.                                          |
| `---> +/-` (Dashed) | **Influence**<br>*(+better / -worse)* | **Influence**  Represents an element's impact on another. Can make the target stronger (`+`) or weaker (`-`). |

### C. Dynamic Relationships (The "When" & "Sequence")
Defines how the architecture evolves over time, handles state changes, and creates value flow.

| Notation Visual             | Handwritten Note Label                    | ArchiMate Standard Equivalent | Meaning & Context                                                                              |
| :---:                       | :---                                      | :---                          | :---                                                                                           |
| `───>` (Solid + Triangle)   | **Will happen next, next step, sequence** | **Triggering**                | Defines a strict temporal or causal relationship. If X happens, Y will absolutely happen next. |
| `---:>` (Dashed + Triangle) | **Value moves to info**                   | **Flow**                      | Defines the movement of value, information, or money between elements.                         |

---
## 3. Key Takeaways for Practical Mapping
*   **Solid vs. Dashed:** 
    * **Solid** lines generally represent **Structural / Realization** relationships (fixed dependencies). 
    * **Dashed** lines generally represent **Dependency / Dynamic** relationships (softer dependencies or time-based events).
*   **Tail = Source:** Always read the arrow from the *tail* to the *head*. The tail's element is the one providing the action (the Power Keeper).
*   **Heart of the Model:** The middle section (`Serving`, `Access`, `Influence`) is where 80% of your business capability mapping will happen. Use them to build your heat maps and gap analysis.
