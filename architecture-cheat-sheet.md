# Architecture cheat sheet
> Communication is more than half of the work of an Enterprise Architecture practice.  
> The real goal is to make your architecture easy enough to understand so that people can make the right decisions.  

## What architecture is:
* Architecture != Tools & Frameworks
* Postponing decisions about Tooling and frameworks
* Focus on customer, not environment

## Architecture trade-offs
* Build vs Buy
* Coding vs Configuration
* Product customization

## Architects ( roles )
* Enterprise
* Solution(System)
* Software(Technical)
* Infrastructure

## Architecture Design
![design]( https://i.ibb.co/P4d0DdQ/architecture-design.png)
1. Analyze Business Drivers, Stakeholders
2. From Assessment (result of evaluation) need to set Goals and more specific Outcomes
3. Gather Requirements from each Outcome
4. prioritize Requirements - find out ASR
5. split them to Functional and NonFunctional Requirements  
   > provide the appropriate level of details 
   > to allow develop/implement the solution.
6. Define [Quality Attributes](https://en.wikipedia.org/wiki/List_of_system_quality_attributes) for NonFunctional Requirements
7. Depict Current Architecture
8. Design Target Architecture ( with Options to achieve MVP )
9. Migration Plan to target architecture

## Agile and Architecture
1. not exhausted UpFront design
2. Documentation only with critical points
3. Main contributors of decisions - Stakeholders
4. Incrementatl design
5. Growing Architecture
6. Value is visible after 2-3 releases

## Architecture context
![architecture context]( https://i.ibb.co/YWth7fR/architecture-context.png)

## Start drawing, drawing focus and purposes
### [Perspectives](http://weblog.tetradian.com/2012/06/06/inside-in-inside-out-outside-in-outside-out/)
* **inside-in**
  > develop a broad understanding of what clean-up would be required    
  > _within each domain in scope_   
* **outside-out**
  > develop a broad understanding of the  
  > _overall business-ecosystem_, in its own terms,   
  > independent of our own organisation  
* **outside-in**
  > develop a broad to detailed understanding of  
  > _how others would interact and transact with our organisation_, from their perspective  
* **inside-out**
  > (usually together with a detailed _inside-in_): develop a detailed architecture     
  > for each domain, each from its own perspective,    
  > drawing on each of _outside-in_ perspectives for guidance    

### Purpose/Viewpoints
inside-in
* **Informing** achieve understanding or obtain commitment.
  > The main goal is to elicit feedback to make sure that the communication is effective.
* **Deciding** support the process of decision-making and often target managers
  > The main goal is to obtain a decision or a choice between several options.
* **Designing** support the design process from initial sketch to detailed design
  > The main goal is usually to define or refine a target.

### Content
* **Overview** - helicopter view on a subject which usually mixes multiples domains 
  > targets decision-makers or enterprise architects.
* **Coherence/Collaboration** - focus on one specific topic, but seen through multiple complementary angles.
  > collaboration between people, processes or tools.
* **Details** - focus on one specific topic and zoom in only one of its aspects.
  > subject matter experts or software engineers.

### Drawing 
* avoid line crossing
* bigger elements will be understood as being more important
* Align elements on a grid and between each other.
* Use whitespace instead of actually using a visual group.


## Waterfall++ - [V-Model system design](https://en.wikipedia.org/wiki/V-model_(software_development))
![v-model](https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Systems_Engineering_Process_II.svg/599px-Systems_Engineering_Process_II.svg.png)

## Design thinking
* emphasize
  * hot points
  * who is asking
  * no tech discussions
  * goals ( business, tech )
* define
  * deep understanding
  * questions
  * use cases
* idea
  * how to 
  * solution architecture
* prototype
  * implementation
* test

## ADR 
[Architecture Decision Records](https://adr.github.io/)
also can be used during development/implementation phase ( not only architecture/design )
* Context
* Decision
* Refused options
* Status
* Assumptions
* Constraints
* Consequences

## resilient architecture
* Timeouts
* Graceful Degradation
* Retries
* Exponential Backoff
* Circuit Breakers

## Application general schema, application demands
* development
* operations
* support
  * L1
  * L2
  * L3
* data migration ( for evolution/revolution )

# Why software architecture
![software architecture](https://i.postimg.cc/D0cMGPPc/software-architecture.png)

## Why to make a documentation:
```mermaid
mindmap
documentation)Documentation(
    {{one common vision}}
        common bird-eye view
        naming conventions
        decrease sketching time for each meeting
    {{part of DefinitionOfDone}}
        visibility
        knowledge sharing
    {{one point of truth}}
        new team member
        existing team memeber
        external teams
    {{interchange responsibility}}
        split hard tasks
        real Agile
```

## Data Architect

### EKI
```
Data + Context = Information
                 Information + Action = Knowledge
                                        Knowledge++ = Experience
```

### Business values of data
* cheaper
* better
* smarter

### Data Strategy
1. caputre & collect
2. clean & prepare
3. $ - capitalize

---
## Examples
![Big Data cluster](https://i.ibb.co/Y8LB999/example-big-data-cluster.png)


## Useful links
* [EIP](https://www.enterpriseintegrationpatterns.com/ramblings.html)
* [C4](https://leanpub.com/visualising-software-architecture)
* [C4 model](https://c4model.com/)
* 97 things every architect should know
* [value proposition template](https://www.strategyzer.com/canvas/value-proposition-canvas)
* [12 factors app](https://12factor.net/)
* [system design descriptions](https://github.com/ByteByteGoHq/system-design-101)
* [design patterns](https://github.com/DovAmir/awesome-design-patterns)
* Quality control ( intentionally in russian due to lack of information in other languages )
  **[семь инструментов контроля качества](https://stump.ru/types/sem-instrumentov-kachestva-sem-novyh-metodov-upravleniya-kachestvom/)**
  * [диаграмма ishikawa](https://ru.wikipedia.org/wiki/%D0%94%D0%B8%D0%B0%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0_%D0%98%D1%81%D0%B8%D0%BA%D0%B0%D0%B2%D1%8B)
  * [контрольная карта](https://ru.wikipedia.org/wiki/%D0%9A%D0%BE%D0%BD%D1%82%D1%80%D0%BE%D0%BB%D1%8C%D0%BD%D0%B0%D1%8F_%D0%BA%D0%B0%D1%80%D1%82%D0%B0_%D0%A8%D1%83%D1%85%D0%B0%D1%80%D1%82%D0%B0)
  * [диаграмма Парето](https://ru.wikipedia.org/wiki/%D0%94%D0%B8%D0%B0%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0_%D0%9F%D0%B0%D1%80%D0%B5%D1%82%D0%BE)
  * [гистограмма](https://ru.wikipedia.org/wiki/%D0%93%D0%B8%D1%81%D1%82%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0)
  * [контрольный лист](https://ru.wikipedia.org/wiki/%D0%9A%D0%BE%D0%BD%D1%82%D1%80%D0%BE%D0%BB%D1%8C%D0%BD%D1%8B%D0%B9_%D1%81%D0%BF%D0%B8%D1%81%D0%BE%D0%BA)
  * [расслоение](https://ru.wikipedia.org/w/index.php?title=%D0%A0%D0%B0%D1%81%D1%81%D0%BB%D0%BE%D0%B5%D0%BD%D0%B8%D0%B5_(%D1%81%D1%82%D1%80%D0%B0%D1%82%D0%B8%D1%84%D0%B8%D0%BA%D0%B0%D1%86%D0%B8%D1%8F)&action=edit&redlink=1)
  * [диаграмма рассеяния](https://ru.wikipedia.org/wiki/%D0%94%D0%B8%D0%B0%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B0_%D1%80%D0%B0%D1%81%D1%81%D0%B5%D1%8F%D0%BD%D0%B8%D1%8F)
  * [дополнительные 7 инструментов контроля качества](https://dzen.ru/a/ZaQAos7VpGMZqodh)
    * диаграмма сродства
    * диаграмма зависимостей ( связей )
    * системная (древовидная) диаграмма
    * матричная диаграмма
    * стрелочная диаграмма
    * диаграмма планирования оценки процесса
    * анализ матричных данных
    * схема потока

## [books](https://www.goodreads.com/shelf/show/software-architecture)
* Clean Architecture ( Robet C. Martin )
* Domain-Driven Design: Tackling Complexity in the Heart of Software
* Software Architecture in Practice ( Len Bass )
* The Software Architect Elevator ( Grehor Hohpe )
* 97 Things Every Software Architect Should Know ( Richard Monson )
* 37 Things One Architect Knows ( Gregor Hohpe )
