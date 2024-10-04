# The Open Group Architecture Framework

[togaf phases](https://pubs.opengroup.org/togaf-standard/adm/chap03.html)    
![togaf phases](https://pubs.opengroup.org/togaf-standard/adm/Figures/a_vis.png)  
![base-target](https://i.postimg.cc/SxzC9f9z/togaf-base-target.png)  

# Archimate
## Examples
* [examples, cookbook, ... ](https://www.hosiaisluoma.fi/blog/category/archimate/)
## Elements

### [Motivation](https://pubs.opengroup.org/architecture/archimate32-doc/ch-Motivation-Elements.html)

#### **Stakeholder**  
* role
* team
* organisation
* group

#### **Driver**
* what motivate to make changes  
* source of influence
* internal or external condition   
Examples:
  * Costs
  * GDPR
  * Market Share
  * Re-organization 
  * Profitability

#### **Assessment**
* outcome of the evaluation of the driver  
* result of analysis of the driver
Examples:
  * Costs are too high
  * Order Process has flaws
  * Customers complain about the helpdesk

#### **Goal**  
end state that stakeholder intend to achieve  
common/general expression with: "increase", "improve", "reduce", "easier"
Examples:
  * Process automation
  * Efficient customer service
  * Increase revenue
  * Occupy high place in ranking system
  * Improve profit

#### **Outcome**  
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

#### **Value**
represent benefit, gain, advantage, artefact (phisycal or virtual!)
Examples:
  * Human Capital
  * Price
  * Partnership
  * Brand

#### **Principle**

#### **Requirement**  
Realise/Implementation of the Outcome - required property of the implementation.
##### Types:
* Functional Requirements
  * functional
    > content of input/output/intermittent information
  * behavioural
    > internal states of the system/sub-systems
  * data
    > structure of input/output information
* Non Functional Requirements ( Quality Attributes )
  * performance
  * security
  * reliability
  * usability
  * maintainability
  * portability
##### Sources:
* Stakeholders
* Documents
* Existing system/application 

#### **Constraint**
  Realise/Implementation of the Outcome - limitation of the implementation.

### [Strategy](https://pubs.opengroup.org/architecture/archimate32-doc/ch-Strategy-Layer.html)

### [Implementation and Migration](https://pubs.opengroup.org/architecture/archimate32-doc/ch-Implementation-and-Migration-Layer.html)

### [Stakeholders, Architecture Views, Viewpoints](https://pubs.opengroup.org/architecture/archimate32-doc/ch-Stakeholders-Architecture-Views-and-Viewpoints.html)

## useful links
* [specification](https://pubs.opengroup.org/architecture/archimate3-doc/)
* [guide](https://www.visual-paradigm.com/guide/archimate/full-archimate-viewpoints-guide/)
* [guide](https://archimate-community.pages.opengroup.org/workgroups/archimate-101/)
* [archimate cheat-sheet](https://gbruneau.github.io/ArchiMate/)
* [how to draw diagrams](https://www.visual-paradigm.com/support/documents/vpuserguide/4455/4409/86421_howtodrawarc.html)
* [blog about modeling](http://renewableplus.blogspot.com/2017/03/modeling-applications-technology-in.html)
* [blog examples](https://www.hosiaisluoma.fi/blog/archimate-examples/)

![when to use archimate](https://archimate-community.pages.opengroup.org/workgroups/archimate-101/part_1/images/why_6.png)
> * Research  -     create notes   
> * Coherence - use/update notes ( a bit create new ) 
> * Details   -        use notes ( a bit update )  
> *after "Details" you can start from the beginning but on another level*
* Metamodel
![togaf metamodel]( https://i.ibb.co/Z1QLbsp/archimate-metamodel.png)    
* Aspects
![togaf aspects]( https://i.ibb.co/42qsSws/archimate-meta-relations.png)    
* Layers
![togaf layers]( https://i.ibb.co/x1C2rhH/archimate-layers.png)    

# Archimate extensions 
## [Archimate to SVG export improvement.](https://github.com/cherkavi/python-utilities/tree/master/xml-archimate2svg)
Update destination SVG with all links from documentation properties ( also add popup hints to elements).

## Archimate with Sequence diagram ( my own invention )
![archimage with sequence diagram](https://i.ibb.co/W5shXP9/archimate-sequence-diagram.png)

## Archimate with Class diagram  ( my own invention )
![archimate with class diagram](https://i.ibb.co/rwH798t/archimate-with-class-diagrams.png)
