# [Motivation View](https://pubs.opengroup.org/architecture/archimate32-doc/ch-Motivation-Elements.html)

## **Stakeholder**  
* role
* team
* organisation
* group

## **Driver**
* what motivate to make changes  
* source of influence
* internal or external condition   
Examples:
  * Costs
  * GDPR
  * Market Share
  * Re-organization 
  * Profitability

## **Assessment**
* outcome of the evaluation of the driver  
* result of analysis of the driver
Examples:
  * Costs are too high
  * Order Process has flaws
  * Customers complain about the helpdesk

## **Goal**  
end state that stakeholder intend to achieve  
common/general expression with: "increase", "improve", "reduce", "easier"
Examples:
  * Process automation
  * Efficient customer service
  * Increase revenue
  * Occupy high place in ranking system
  * Improve profit

## **Outcome**  
Realise/Implementation of the goal (in most cases),  
that is going to be achieved.  
Unambiguously specify the end result - measurable result.
Influence on the Goal can be positive and Negative.  
Difference between goals and outcomes: not all outcomes lead to the intended results.
Examples:
  * Robots instead of people 
  * Customer satisfaction increased in 15%
  * revenue should be at least 12% per year
  * occupy at least 3-rd place in ranking system
  * increase profit by 10%  

## **Value**
represent benefit, gain, advantage, artefact (phisycal or virtual!)
Examples:
  * Human Capital
  * Price
  * Partnership
  * Brand

## **Requirement**, **Principle**, **Constraint**
Realise/Implementation of the Outcome - demands/limitations of the implementation.

### Types:
* Functional Requirements (FR == UseCases) ( "Shift"==FR + nFR? )
  * functional
    > content of input/output/intermittent information
  * behavioural
    > internal states of the system/sub-systems
  * data
    > structure of input/output information
* Non Functional Requirements ( Quality Attributes ) ( "Lift" == nFR )
  * performance
  * security
  * reliability
  * usability
  * maintainability
  * portability

### Sources:
* Stakeholders
* Documents
* Existing system/application 

# [Strategy View](https://pubs.opengroup.org/architecture/archimate32-doc/ch-Strategy-Layer.html)

## course of actions
how are you going to **achieve** that ?

## Business Capability
> what are you **able** to do ?
**Goal:** Bridge the gap between Business Strategy and Tech Strategy to define actionable, unique, and atomic capabilities.  
Business Strategy and Tech strategy hasve different goals, different languages in communication between diff group of people. 
The foundational challenge is aligning **Business Strategy** with **Technology Strategy**.

| Aspect       | Business Strategy                       | Technology Strategy                      |
| :---         | :---                                    | :---                                     |
| **Focus**    | Course of actions to achieve goals      | Execution, platforms, and infrastructure |
| **Language** | Different language & goals              | Different language & goals               |
| **Goal**     | Align to create a **New Business View** | Support the Business View                |

Don't confuse **Capabilities** with **Processes**:

| Concept        | Part of Speech | Example                            | Nature                                           |
| :---           | :---           | :---                               | :---                                             |
| **Capability** | **Noun**       | Procurement, Customer Management   | **Static / Non-changeable** (Unique & Atomic)    |
| **Process**    | **Verb**       | Develop Product, Procure Materials | Dynamic, changes over time                       |

> ⚠️ **Crucial Rule:** Capabilities are **unique**, **atomic**, and should **not** be tied to your organizational structure. 
> They represent "what" you can do, regardless of who does it.
> It is not a strategy ( can be changed at any time )

### Step-by-Step Process: Map, Rate, Uplift

This is a 3-step framework for creating a strategic capability map.

#### Step 1: Map (Identify Structure)
*   Build a hierarchical capability breakdown.
*   **Level 0:** Highest strategic level.
*   **Level 1:** Core business areas.
*   **Level 2:** Specific sub-capabilities.
*   *Rule:* Stop at **Level 3 or 4**. Going deeper than Level 4 usually moves into specific operational tasks or technology implementations (which changes too frequently).

#### Step 2: Rate (Heat Map Analysis)
Evaluate your current capabilities against your business strategy.

*   **Question:** *How well do they support the organization?*
*   **Visual:** Use a colored "Heat Map".
*   **Priority Scale:**
    *   `?` = Not Implemented
    *   `🔴 High` = Critical, high priority
    *   `🟡 Medium` = Needed, manageable priority
    *   `🟢 Low` = Low immediate need

#### Step 3: Uplift (Gap Analysis)
*   Identify **missed elements**.
*   Analyze what needs to be built, bought, or changed to support the new Business Strategy.

---
### Roadmapping: From Business to Technology

Once you have the rated map, create an actionable roadmap.

---
### Business Roadmap
Sequence the evolution of your capabilities over time. Use the rating scale to show progression:

`H (High) ➔ H (High) ➔ M (Medium) ➔ M (Medium) ➔ ? (Unimplemented) ➔ M (Medium)`

The Business Roadmap must **map to** the Technology Roadmap.

### Technology Roadmap
*   Define how technology capabilities will enable the business capabilities.
*   **Example:** `T1 (Tech 1) ➔ T2 (Tech 2) ➔ T3 (Tech 3)`
*   *Rule:* Business Roadmap drives the Technology Roadmap.

---
### Tips for Successful Implementation

*   🌱 **Start small.** Don't try to map the entire enterprise at once.
*   🎯 **Find a good Use Case.** Pick a specific pain point to validate the model.
*   💰 **Secure Resources.** You need both a **Business Sponsor** and a **budget**.
*   ✋ **Stop at Level 3/4.** Do not over-granulate.
*   🗣️ **Use Business Language.** The capabilities must be defined by the *Business Owners*, not IT. (e.g., Use "Customer Acquisition" instead of "Lead Gen System").

---
### Quick Glossary
| Term           | Meaning                                                                                    |
| :---           | :---                                                                                       |
| **Capability** | A static, unique, and atomic ability of an organization. (Noun)                            |
| **Process**    | A dynamic sequence of actions. (Verb)                                                      |
| **Heat Map**   | A visual rating system (High, Medium, Low) to show maturity/support level.                 |
| **Uplift**     | The action of finding and filling gaps to support the strategy.                            |
| **Level 3/4**  | The recommended depth for capability mapping to avoid getting lost in operational details. |

---
### Self-Check & Analysis of Source Notes
*   **Logic Check:**
    *   The core logic is sound. Capabilities are "what" (nouns) and are static; Processes are "how" (verbs) and are fluid. The notes explicitly warn against tying capabilities to org charts—this is a classic Enterprise Architecture mistake.
    *   The differentiation between Business and Tech strategy as having "different languages" is the central reason *why* a capability map is needed as a translation layer.
*   **Process Integrity:**
    *   The `Map -> Rate -> Uplift` framework is a simplified, pragmatic interpretation of TOGAF's Phase B (Business Architecture).
    *   The roadmap advice (`Business Roadmap -> Technology Roadmap`) aligns perfectly with standard architecture practices.
*   **Actionability:**
    *   The warning "Don't go deeper than 3/4" is excellent practical advice. In large enterprises, getting stuck in Level 5 or 6 details derails capability mapping projects.
    *   The emphasis on "Use Business Language" is a strong soft-skill directive, ensuring that the technical team translates their needs into terms the business stakeholders care about.
*   **Note on Nomenclature:**
    *   The note mentions "TOGAF Capability Frameworks -> 2G / YT Cap. Map. Mastery in 15 min". This suggests the source is a rapid educational overview (likely from a "Youtube" video) aiming to distill complex TOGAF/ArchiMate theory into a practical 15-minute framework.


## resource
what do you **need** for that ?

## value stream
what is the **results** ?


# [Business Layer](https://pubs.opengroup.org/architecture/archimate32-doc/ch-Business-Layer.html)
Start of understanding existing business Model can be started from:
* Operational Model ( part of capability model)
* Capability Model 
  * Map capability ( Top->Medium->Detailed levels )
  * Rate capability ( Green, Orange, Red )
  * Identify capability uplifts
  * Prioritise capabilities 
  * Create business roadmap 
  * Create technology roadmap

# [Application Layer](https://pubs.opengroup.org/architecture/archimate32-doc/ch-Application-Layer.html)

# [Technology Layer](https://pubs.opengroup.org/architecture/archimate32-doc/ch-Technology-Layer.html)

# [Implementation and Migration view](https://pubs.opengroup.org/architecture/archimate32-doc/ch-Implementation-and-Migration-Layer.html)

# [Stakeholders, Architecture Views, Viewpoints](https://pubs.opengroup.org/architecture/archimate32-doc/ch-Stakeholders-Architecture-Views-and-Viewpoints.html)
