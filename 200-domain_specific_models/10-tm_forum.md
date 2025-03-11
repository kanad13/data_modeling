# On this page

- **This page serves as an introduction to the topic of TM Forum's SID.**
- To check out other related topics, click on the links from the diagram below.
- To continue with the current topic, scroll down to read more.

```mermaid
graph LR
    %% Main node
    DM["Data Modeling Approaches"]
    style DM fill:#e5e5e5,stroke:#333,stroke-width:2px
    click DM href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/05-overview_of_data_modeling_concepts.md" "Click for more information"

    %% First level connections
    DM --> RDM
    DM --> GDM
    DM --> SDM
    DM --> DDM

    %% Main approaches - Parent Level 1
    RDM["Relational Data Modeling"]
    GDM["Graph Data Modeling"]
    SDM["Semantic Data Modeling"]
    DDM["Document-oriented Data Modeling"]
    style RDM fill:#ffebee,stroke:#d32f2f,stroke-width:2px
    style GDM fill:#e3f2fd,stroke:#1565c0,stroke-width:2px
    style SDM fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    style DDM fill:#f3e5f5,stroke:#6a1b9a,stroke-width:2px
    click RDM href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/10-relational_data_modeling.md" "Click for more information"
    click GDM href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/20-graph_data_modeling.md" "Click for more information"
    click SDM href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/30-semantic_data_modeling.md" "Click for more information"
    click DDM href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/40-json_based_modeling.md" "Click for more information"

    %% First level Implementations - Parent Level 2
    Tables["Tables & SQL"]
    NodesEdges["Nodes & Edges"]
    Documents["JSON Documents"]
    RDM --> Tables
    GDM --> NodesEdges
    DDM --> Documents
    style Tables fill:#ffebee,stroke:#d32f2f,stroke-width:2px
    style NodesEdges fill:#e3f2fd,stroke:#1565c0,stroke-width:2px
    style Documents fill:#f3e5f5,stroke:#6a1b9a,stroke-width:2px
    click Tables href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/10-relational_data_modeling.md" "Click for more information"
    click NodesEdges href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/20-graph_data_modeling.md" "Click for more information"
    click Documents href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/40-json_based_modeling.md" "Click for more information"

    %% Tools and Technologies & Semantic specifics - Parent Level 3
    ERTools["ER Diagram Tools"]
    UMLTools["UML Tools"]
    TMFSID["TMForum SID"]
    GraphTools["Graph Database Tools"]
    DocumentTools["Document DB Tools"]
    RDF["RDF - Resource Description Framework"]
    RDFS["RDFS - RDF Schema"]
    OWL["OWL - Web Ontology Language"]
    Tables --> ERTools
    Tables --> UMLTools
    Tables --> TMFSID
    NodesEdges --> GraphTools
    Documents --> DocumentTools
    SDM --> RDF
    SDM --> RDFS
    SDM --> OWL
    style ERTools fill:#ffebee,stroke:#d32f2f,stroke-width:2px
    style UMLTools fill:#ffebee,stroke:#d32f2f,stroke-width:2px
    style TMFSID fill:#ffcb6b,stroke:#d32f2f,stroke-width:2px
    style GraphTools fill:#e3f2fd,stroke:#1565c0,stroke-width:2px
    style DocumentTools fill:#f3e5f5,stroke:#6a1b9a,stroke-width:2px
    style RDF fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    style RDFS fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    style OWL fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    click ERTools href "https://github.com/kanad13/data_modeling/blob/master/120-data_modeling_tools/10-er_diagram_tools.md" "Click for more information"
    click UMLTools href "https://github.com/kanad13/data_modeling/blob/master/120-data_modeling_tools/20-uml_tools.md" "Click for more information"
    click TMFSID href "https://github.com/kanad13/data_modeling/blob/master/200-domain_specific_models/10-tm_forum.md" "Click for more information"
    click GraphTools href "https://github.com/kanad13/data_modeling/blob/master/120-data_modeling_tools/30-graph_data_modeling_tools.md" "Click for more information"
    click DocumentTools href "https://github.com/kanad13/data_modeling/blob/master/120-data_modeling_tools/50-json_based_modeling_tools.md" "Click for more information"
    click RDF href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/31-resource_description_framework.md" "Click for more information"
    click RDFS href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/32-resource_description_framework_schema.md" "Click for more information"
    click OWL href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/33-web_ontology_language.md" "Click for more information"

    %% Semantic Data Modeling specifics - Deeper Level 4
    Triples["RDF Triples"]
    RDFSVocabulary["RDFS Vocabulary"]
    SHACL["SHACL - Shapes Constraint Language"]
    RDF --> Triples
    RDFS --> RDFSVocabulary
    OWL --> SHACL
    style Triples fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    style RDFSVocabulary fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    style SHACL fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    click Triples href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/31-resource_description_framework.md" "Click for more information"
    click RDFSVocabulary href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/32-resource_description_framework_schema.md" "Click for more information"
    click SHACL href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/34-shapes_constraint_language.md" "Click for more information"
```

# TM Forum's Information Framework

## Introduction

- The TM Forum's Information Framework (SID, eTOM, and TAM) is a comprehensive set of standards and guidelines for the telecommunications industry.
- These components are closely related to the data modeling [techniques](../100-data_modeling_approaches) and [tools](../120-data_modeling_tools) discussed in the other folders in this repository.
- Here's how they are co-related:
  - **SID (Shared Information/Data Model):**
    - Primarily based on UML and entity-relationship concepts.
    - Uses a hierarchical information model that can be implemented in relational databases.
    - Often used for telecommunications data modeling that gets implemented in SQL databases.
  - **eTOM (Enhanced Telecom Operations Map):**
    - Provides a comprehensive business process framework.
    - Can be mapped to various data modeling techniques to ensure that data models support business processes effectively.
  - **TAM (Telecom Applications Map):**
    - Blueprints application alignment with business functions.
    - Ensures that data models are aligned with the applications that use them.
  - **Open Digital Architecture (ODA) and TM Forum Open APIs:**
    - Facilitate the integration and interoperability of different systems and applications.
    - Ensure that data models are compatible with industry standards and can be easily integrated with other systems.

## In this Document

- **This document explains**
  - TM Forum's Information Framework components (SID, eTOM, and TAM)
  - How these components work together
  - Open Digital Architecture (ODA)
  - TM Forum Open APIs
- **The goal is**
  - to provide a technical understanding of these frameworks and
  - their practical implementation in telecom systems.
- **Structure of this document**
  - Introduction to TM Forum
  - Information Framework
    - SID
    - eTOM
    - TAM
  - ODA and Open APIs

## Introduction to TM Forum

- TM Forum drives digital transformation in telecommunications.
- It provides industry-standard frameworks, tools, and best practices for service providers and suppliers in the telecom/digital services industry.
- It helps organizations modernize systems, ensure business continuity, and reduce risks during digital transformation.

## TM Forum - Information Framework

- **About the Information Framework**
  - TM Forum offers industry-standard frameworks for integrated management of telecom operations and IT infrastructure.
- **Components of the Information Framework**
  - `SID (Shared Information/Data Model)` Standardizes data definitions for a common language across systems.
  - `eTOM (Enhanced Telecom Operations Map)` Provides a comprehensive business process framework.
  - `TAM (Telecom Applications Map)` Blueprints application alignment with business functions.
- **Interactive Exploration**
  - Access the Information Framework [here](https://www.tmforum.org/oda/moda/)
  - ![](/900-assets/tm_forum-01.png)

### Integration of SID, eTOM, and TAM

- **Together, SID, eTOM, and TAM provide a comprehensive view of telecom operations**
  - eTOM defines processes
  - SID defines data
  - TAM defines applications
- **TAM**
  - Identifies applications implementing eTOM processes
- **SID**
  - Defines data used by TAM applications
- **eTOM**
  - Defines processes that TAM applications implement

### Analogy using Data Modeling Levels

- **Conceptual Data Model**
  - Focuses on the "big picture": what entities exist and how they relate.
  - Remains free of technical details, ensuring it is technology agnostic.
- **Logical Data Model**
  - Digs into the details: defines the structure, attributes, data types, and relationships.
  - Acts as a bridge between business requirements and technical implementation.
- **Physical Data Model**
  - Details how the logical model is implemented using a specific technology.
  - Specifies database features such as tables, columns, indexes, and constraints.

| Data Model Type | Information Framework Component | Primary Purpose                                                                       |
| --------------- | ------------------------------- | ------------------------------------------------------------------------------------- |
| **Conceptual**  | **SID**                         | Defines WHAT information the business manages (business concepts and data entities)   |
| **Logical**     | **eTOM**                        | Defines HOW the business operates (business processes and operational workflows)      |
| **Physical**    | **TAM**                         | Defines WHAT application capabilities are needed (application functions and features) |

### SID

- **What is SID?**
  - A standardized data model for the telecommunications industry.
  - Provides a common language for data definitions, ensuring consistent understanding and usage across systems.
  - Enables interoperability and integration of systems, reducing complexity and improving efficiency.
- **SID - Domain**
  - `Definition`
    - A high-level grouping of related business areas that represent major functional parts of a telecom business.
    - SID organizes telecom business concepts in a structured hierarchy.
  - `Practical Analogy`
    - Think of them as the "departments" or "subject areas" in a company.
  - `SID Context Example`
    - Customer Domain, Product Domain, Service Domain, Resource Domain
  - ![](/900-assets/tm_forum-02.png)
  - `SID domains`
    - SID is organized into domains, which represent major functional areas of the telecom business.
    - These domains provide a logical grouping for related business concepts.

```mermaid
graph TD
    SID[SID Model Domains]
    Customer[Customer Domain]
    Product[Product Domain]
    Service[Service Domain]
    Resource[Resource Domain]

    SID --> Customer
    SID --> Product
    SID --> Service
    SID --> Resource

    Customer --> CustomerAccount[Customer Account]
    Customer --> CustomerOrder[Customer Order]
    Customer --> CustomerBill[Customer Bill]

    Product --> ProductOffering[Product Offering]
    Product --> ProductSpecification[Product Specification]

    Service --> ServiceSpecification[Service Specification]
    Service --> ServiceConfiguration[Service Configuration]

    Resource --> LogicalResource[Logical Resource]
    Resource --> PhysicalResource[Physical Resource]
```

- **SID - Abstract Business Entity (ABE)**
  - `Definition`
    - Drilling down into a Domain, brings us to the Abstract Business Entity (ABE).
    - ABE is a subdivision within a Domain, grouping together related Entities within a Domain to further organize the model.
  - `Practical Analogy`
    - "Folder" within a Department
  - `SID Context Example`
    - In image above, within each Domain rectangle, smaller colored rectangles labeled "ABE" represent Abstract Business Entities.
- **SID - Business Entity (BE)**
  - `Definition`
    - A fundamental building block of the SID, representing a distinct "thing," "concept," or "object" in the business domain that we need to store information about.
  - `Practical Analogy`
    - Entities are like the "nouns" in the business language.
  - `SID Context Example`
    - CustomerBillingAccount, CustomerAccount, CustomerBill (yellow boxes in diagrams)
  - ![](/900-assets/tm_forum-04.png)
- **SID - Attribute**
  - `Definition`
    - A characteristic or property of an Entity, describing the data elements associated with an Entity.
  - `Practical Analogy`
    - Attributes are like the "adjectives" that describe the "nouns" (Entities).
  - `SID Context Example`
    - creditLimit, pin in CustomerBillingAccount (listed under "Attributes" tab)
  - ![](/900-assets/tm_forum-03.png)
- **SID - Relationship (or Association)**
  - `Definition`
    - A connection or link between two or more Entities, describing how Entities are related in the business context.
  - `Practical Analogy`
    - Relationships are like the "verbs" that connect "nouns."
  - `SID Context Example`
    - Lines connecting Entity boxes in diagrams, labeled with relationship type and cardinality.
    - CustomerBillingAccount _described by_ CustomerBill, PartyRole _plays_ Customer
  - ![](/900-assets/tm_forum-04.png)

| Term              | Definition                                                       | Practical Analogy                      | SID Context Example                                                            |
| ----------------- | ---------------------------------------------------------------- | -------------------------------------- | ------------------------------------------------------------------------------ |
| **Domain**        | High-level business area grouping related concepts.              | "Department" in a company              | Customer Domain, Product Domain, Service Domain, Resource Domain               |
| **Package** (ABE) | Subdivision within a Domain, grouping related Entities.          | "Folder" within a Department           | Customer Management ABE, Billing ABE                                           |
| **Entity**        | A distinct "thing," "concept," or "object" in the business.      | "Noun"                                 | CustomerBillingAccount, CustomerAccount, CustomerBill                          |
| **Attribute**     | A characteristic or property of an Entity.                       | "Adjective"                            | creditLimit, pin in CustomerBillingAccount                                     |
| **Relationship**  | A connection or link between Entities.                           | "Verb"                                 | CustomerBillingAccount _described by_ CustomerBill, PartyRole _plays_ Customer |
| **Class**         | Often used interchangeably with Entity, sometimes more abstract. | "Blueprint" (in object-oriented terms) | CustomerBillingAccount (concrete entity in the diagram)                        |
| **Aggregate**     | Collection of related Entities treated as a unit.                | "Document with embedded sections"      | CustomerBillingAccount with related entities and connections                   |

### eTOM

- **What is eTOM?**
  - `Definition`
  - A comprehensive `business process framework` for telecom service providers.
  - Provides a standardized view of all business processes required to run a telecom operation.
  - `Practical Analogy`
    - Blueprint for Business Processes
  - `eTOM Context Example`
    - eTOM (overall structure)
  - ![](/900-assets/tm_forum-05.png)
- **eTOM Level 1 Process Area**
  - `Definition`
    - Major category of business processes, representing a high-level overview of the entire business process landscape.
  - `Practical Analogy`
    - Department
  - `eTOM Context Example`
    - Operations, Strategy, Enterprise Management
  - ![](/900-assets/tm_forum-06.png)

```mermaid
graph TD
    eTOM[eTOM Framework Domains]
    SIP[Strategy, Infrastructure & Product]
    OPS[Operations]
    EM[Enterprise Management]

    eTOM --> SIP
    eTOM --> OPS
    eTOM --> EM

    OPS --> Fulfillment[Fulfillment]
    OPS --> Assurance[Assurance]
    OPS --> Billing[Billing & Revenue]

    Fulfillment --> OrderHandling[Order Handling]
    Fulfillment --> ServiceConfig[Service Configuration]

    Assurance --> ProblemMgmt[Problem Management]
    Assurance --> ServiceQuality[Service Quality Management]

    Billing --> BillPrep[Bill Preparation]
    Billing --> Collections[Collections]
```

- **eTOM Level 2 Process Area**
  - `Definition`
    - Sub-category of processes within a Level 1 area, representing key functional domains within each broader category.
  - `Practical Analogy`
    - Division within a Department
  - `eTOM Context Example`
    - Fulfillment, Assurance, Billing (within Operations)
  - ![](/900-assets/tm_forum-07.png)
- **eTOM Level 3 Process Grouping**
  - `Definition`
    - Group of related processes within a Level 2 area, providing even more detail.
  - `Practical Analogy`
    - "Section within a Division"
  - `eTOM Context Example`
    - Manage Customer Order Placement, Manage Customer Order Fulfillment
  - ![](/900-assets/tm_forum-08.png)
- **eTOM Level 4 Process**
  - `Definition`
    - Specific set of activities to achieve a business goal, representing the most granular level of detail.
  - `Practical Analogy`
    - "Process/Task"
  - `eTOM Context Example`
    - Capture Customer Order, Issue Customer Order

| Term                          | Definition                                            | Practical Analogy                  | eTOM Context Example                                               |
| ----------------------------- | ----------------------------------------------------- | ---------------------------------- | ------------------------------------------------------------------ |
| eTOM Framework                | Standard business process framework for telecoms      | "Blueprint for Business Processes" | eTOM (overall structure)                                           |
| eTOM Level 1 Process Area     | Major category of business processes                  | "Department"                       | Operations, Strategy, Enterprise Management                        |
| eTOM Level 2 Process Area     | Sub-category of processes within a Level 1 area       | "Division within a Department"     | Fulfillment, Assurance, Billing (within Operations)                |
| eTOM Level 3 Process Grouping | Group of related processes within a Level 2 area      | "Section within a Division"        | Manage Customer Order Placement, Manage Customer Order Fulfillment |
| eTOM Level 4 Process          | Specific set of activities to achieve a business goal | "Process/Task"                     | Capture Customer Order, Issue Customer Order                       |

### TAM

- **What is TAM?**
  - `Definition`
    - A business-oriented view of the telecom application landscape.
    - Outlines the functional capabilities that telecom applications should provide to support the business processes defined in eTOM and manage the data defined in SID.
  - `Practical Analogy`
    - "Software Catalog"
  - `TAM Context Example`
    - TAM (overall structure)
  - ![](/900-assets/tm_forum-09.png)
- **TAM Level 1 Application Area (or Layers)**
  - `Definition`
    - Major category of application functionality, representing high-level application domains. These are also commonly referred to as _TAM Layers_.
  - `Practical Analogy`
    - "Application Domain" or "Application Layer"
  - `TAM Context Example`
    - Customer-Facing Applications, Business Management Applications, Resource-Facing Applications, Infrastructure Applications (often grouped into layers)
  - ![](/900-assets/tm_forum-10.png)

```mermaid
graph TD
    TAM[TAM Framework Layers]
    CFA[Customer-Facing Applications]
    BMA[Business Management Applications]
    RFA[Resource-Facing Applications]
    INFRA[Infrastructure Applications]

    TAM --> CFA
    TAM --> BMA
    TAM --> RFA
    TAM --> INFRA

    CFA --> CRM[CRM Systems]
    CFA --> SelfService[Self-Service Portals]

    BMA --> BillingSystem[Billing Systems]
    BMA --> OrderManagement[Order Management]
    BMA --> ProductCatalog[Product Catalog]

    RFA --> ServiceManagement[Service Management]
    RFA --> NetworkManagement[Network Management]

    INFRA --> Integration[Integration Platforms]
    INFRA --> DataMgmt[Data Management]
```

- **TAM Level 2 Application Area**
  - `Definition`
    - More specific functional grouping of applications within a Level 1 Area, representing specific application functional areas.
  - `Practical Analogy`
    - "Application Functional Area"
  - `TAM Context Example`
    - Customer Order Management, Customer Information Management
  - ![](/900-assets/tm_forum-11.png)
- **TAM Application**
  - `Definition`
    - Specific software system or functional module, representing a concrete software component with a defined function.
  - `Practical Analogy`
    - "Software Application/Module"
  - `TAM Context Example`
    - Customer Order Acceptance, Customer Order Enrichment
  - ![](/900-assets/tm_forum-12.png)

| Term                         | Definition                                                              | Practical Analogy             | TAM Context Example                                        |
| ---------------------------- | ----------------------------------------------------------------------- | ----------------------------- | ---------------------------------------------------------- |
| TAM (Functional Framework)   | Application framework for telecoms                                      | "Software Catalog"            | TAM (overall structure)                                    |
| TAM Level 1 Application Area | Major category of application functionality                             | "Application Domain"          | Customer Domain, Product Domain, Service Domain            |
| TAM Level 2 Application Area | More specific functional grouping of applications within a Level 1 Area | "Application Functional Area" | Customer Order Management, Customer Information Management |
| TAM Application              | Specific software system or functional module                           | "Software Application/Module" | Customer Order Acceptance, Customer Order Enrichment       |

## TM Forum - ODA and Open APIs

- Information Framework provides the `conceptual foundation` for telecom operations.
- TM Forum further promotes interoperability and agility through standardized APIs and data models
- For this reason, TM Forum has developed the
  - `Open Digital Architecture (ODA)`
  - `Open APIs`
- Next sections will cover these two topics in detail.

### Open Digital Architecture (ODA)

- **What is ODA?**
  - Provides a framework for integrating various systems and applications within the telecom ecosystem.
  - Breaks down complex systems into smaller, reusable parts.
  - It replaces traditional operations and business support systems (OSS/BSS) with a new approach that simplifies your design, modernizes your build, and automates your operation.
  - ![](/900-assets/tm_forum-13.png)
- **Interactive explorer**
  - Find it [here](https://www.tmforum.org/oda/)
  - ![](/900-assets/tm_forum-14.png)

### TM Forum Open APIs

- **What are Open APIs?**
  - TM Forum Open APIs are standardized REST APIs with JSON payloads specifically designed for telecom operations.
  - They provide practical, well-documented, and widely adopted interfaces for various telecom business functions.
- **Open APIs and the Information Framework**
  - `SID Implementation` APIs expose SID data in a standardized format, allowing systems to exchange information based on the common data model.
  - `eTOM Enablement` API operations are designed to support eTOM business processes, facilitating standardized process execution across different systems.
  - `TAM Connectivity` TAM applications can connect and interact with each other through Open APIs, enabling a modular and interoperable application landscape.
- **More details**
  - Find them [here](https://www.tmforum.org/oda/open-apis/open-api-dashboard/)
  - ![](/900-assets/tm_forum-15.png)
  - ![](/900-assets/tm_forum-16.png)
