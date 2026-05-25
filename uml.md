# UML 

## UML Profiles and extensions 

### UML EDOC
EDOC (Enterprise Distributed Object Computing) - UML Profile.  
Create visual map for ideas, so the development team knows exactly what to code.  
The EDOC Solution: It shifts the focus to "Roles" and "Ports." It asks: What is this service expected to do in this specific business process, and how does it plug into the rest of the ecosystem?
EDOC provides a way to model **collaborations** rather than just static objects.

* **The Problem:** Traditional UML classes focus on internal structure (data and methods).
* **The EDOC Solution:** It shifts the focus to **"Roles"** and **"Ports."** It asks: *What is this service expected to do in this specific business process, and how does it plug into the rest of the ecosystem?*

Instead of drawing monolithic class diagrams, think in "EDOC Terms":
* **Identify Communities:** Group your microservices or business units into "Communities" (bounded contexts).
* **Define Interaction Roles:** Don't just draw a box for "OrderService." Define the *role* it plays in the "Checkout Process" (e.g., the *Validator*, the *PaymentProcessor*, or the *Notifier*).
* **Focus on Ports & Connectors:** Stop using generic lines. Define the *interface* (Port) and the *interaction protocol* (Connector—e.g., REST, gRPC, Kafka topic). This makes your architecture resilient to change because you can swap the internal implementation of a "service" as long as the "port" remains the same.

If you want to adopt this style of thinking, use these visual patterns:
| Concept           | The "EDOC" Way to View It                    | Modern Translation                         |
| ---               | ---                                          | ---                                        |
| **Collaboration** | A set of roles working together.             | A Saga, a workflow, or a business process. |
| **Role**          | What a component does in a specific context. | Service interface or Consumer/Producer.    |
| **Port**          | The boundary of a component.                 | API endpoint, Message queue consumer.      |
| **Connector**     | The glue between components.                 | HTTP/JSON, Protobuf, Pub/Sub events.       |


### UML-RT (UML for Real-Time)
- **Purpose**: Real-time and embedded systems modeling
- **Key Features**: Capsules, ports, protocols, state machines with timing
- **Applications**: Telecommunications, automotive, aerospace
- **Links**: 
  - [UML-RT Profile - Eclipse](https://www.eclipse.org/papyrus-rt/)
  - [UML-RT Documentation](https://wiki.eclipse.org/Papyrus-RT)

### Object Parallel Computing (OPC, OPC UA)
- **Purpose**: Parallel and distributed object-oriented systems
- **Key Features**: Parallel objects, synchronization, distribution
- **Applications**: High-performance computing, distributed systems
- **Links**:
  - [OPC Foundation](https://opcfoundation.org/)
    - https://reference.opcfoundation.org/DI/v102/docs/4.2.1/
  - [OPC UA](https://github.com/model-UA/uml-to-opcua)

### UML4ODP (Open Distributed Processing) RM-ODP (Reference Model of Open Distributed Processing)
- **Purpose**: Distributed systems architecture
- **Key Features**: Viewpoints, transparencies, policies
- **Applications**: Large-scale distributed systems
- **Links**:  
  - [use UML for ODP](https://cdn.standards.iteh.ai/samples/68641/df5d5236c264473cabc4528c3c866291/ISO-IEC-19793-2015.pdf)
  - [sparx odp library](https://sparxsystems.com/products/3rdparty/odp)
  - Modeling the ODP computational viewpoint with UML 2.0

### UMLsec
- **Purpose**: Security-critical systems
- **Key Features**: Security stereotypes, threat modeling, access control
- **Applications**: Secure system design, security analysis
- **Links**:
  - [UMLsec Wikipedia](https://en.wikipedia.org/wiki/UMLsec)
  - [UMLsec Research Paper](https://www.researchgate.net/publication/220868409_UMLsec_Extending_UML_for_secure_systems_development)
  - [Springer Link](https://link.springer.com/chapter/10.1007/3-540-45800-X_32)

### Defence Extension UML DoDAF
- **Purpose**: Security-critical systems
- **Key Features**: Security stereotypes, threat modeling, access control
- **Applications**: Secure system design, security analysis
- **Links**: 
  - [DoDAF Overview](https://dodaf.net)
  - [UML Security Extensions](https://www.omg.org/spec/UML/)

### Defence Extension UML MODAF
- **Purpose**: Security-critical systems
- **Key Features**: Security stereotypes, threat modeling, access control
- **Applications**: Secure system design, security analysis
- **Links**: 
  - [MODAF Overview](https://www.gov.uk/government/publications/modaf)
  - [UML Security Extensions](https://www.omg.org/spec/UML/)


## Official Organizations and Standards

### OMG (Object Management Group)
- **Main Site**: [https://www.omg.org/](https://www.omg.org/)
- **UML Specifications**: [https://www.omg.org/spec/UML/](https://www.omg.org/spec/UML/)
- **UML Profile Category**: [https://www.omg.org/spec/category/uml-profile](https://www.omg.org/spec/category/uml-profile)

### ISO/IEC Standards
- **ISO/IEC 19505**: [UML Standard](https://www.iso.org/standard/32624.html)
- **ISO Standards Search**: [https://www.iso.org/standards.html](https://www.iso.org/standards.html)

### IEEE Standards
- **IEEE Computer Society**: [https://www.computer.org/](https://www.computer.org/)
- **IEEE Xplore**: [https://ieeexplore.ieee.org/](https://ieeexplore.ieee.org/)


## Tool Support

### Commercial Tools
- **Visual Paradigm**: [https://www.visual-paradigm.com/](https://www.visual-paradigm.com/)
- **Enterprise Architect**: [https://sparxsystems.com/](https://sparxsystems.com/)
- **MagicDraw**: [https://www.3ds.com/products-services/catia/products/no-magic/](https://www.3ds.com/products-services/catia/products/no-magic/)
- **Modelio**: [https://www.modeliosoft.com/](https://www.modeliosoft.com/)

### Open Source Tools
- **Eclipse Papyrus**: [https://www.eclipse.org/papyrus/](https://www.eclipse.org/papyrus/)
- **PlantUML**: [https://plantuml.com/](https://plantuml.com/)
- **StarUML**: [https://staruml.io/](https://staruml.io/)
- **ArgoUML**: [http://argouml.tigris.org/](http://argouml.tigris.org/)
