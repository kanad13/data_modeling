# Introduction to Data Modeling

## Overview of the Repository

- This repository serves as an introduction to the topic of data modeling.
- It contains documents that provide insights into various data modeling techniques, tools, and industry standards.

## Topics Covered

- **Click on any of the links in the boxes to explore the respective topics**:

```mermaid
graph LR
    %% Main node
    DM[Data Modeling Approaches]

    %% Main approaches
    RDM[Relational Data Modeling]
    GDM[Graph Data Modeling]
    SDM[Semantic Data Modeling]
    DDM[Document-oriented Data Modeling]

    %% First level connections
    DM --> RDM
    DM --> GDM
    DM --> SDM
    DM --> DDM

    %% Implementations
    RDM --> Tables[Tables & SQL]
    GDM --> NodesEdges[Nodes & Edges]
    SDM --> Triples[RDF Triples]
    DDM --> Documents[JSON Documents]

    %% Tools and Technologies
    Tables --> ERTools[ER Diagram Tools]
    Tables --> UMLTools[UML Tools]
    Tables --> TMFSID[TMForum SID]
    NodesEdges --> GraphTools[Graph Database Tools]
    Triples --> SemanticTools[Semantic Web Tools]
    Documents --> DocumentTools[Document DB Tools]

    %% Semantic Data Modeling specifics
    SDM --> RDF[RDF - Resource Description Framework]
    SDM --> RDFS[RDFS - RDF Schema]
    SDM --> OWL[OWL - Web Ontology Language]
    SDM --> SHACL[SHACL - Shapes Constraint Language]
    OWL --> SHACL
    SHACL --> Validation[Validation & Data Quality]

    %% Styling main node
    style DM fill:#ffec5c,stroke:#555,stroke-width:2px

    %% Level 1 - Main approach nodes (darker shades)
    style RDM fill:#d580ff,stroke:#333,stroke-width:1px
    style GDM fill:#8080ff,stroke:#333,stroke-width:1px
    style SDM fill:#80d580,stroke:#333,stroke-width:1px
    style DDM fill:#ff8080,stroke:#333,stroke-width:1px

    %% Level 2 - Implementation nodes (medium shades)
    style Tables fill:#e6b3ff,stroke:#333,stroke-width:1px
    style NodesEdges fill:#b3b3ff,stroke:#333,stroke-width:1px
    style Triples fill:#b3e6b3,stroke:#333,stroke-width:1px
    style Documents fill:#ffb3b3,stroke:#333,stroke-width:1px
    style RDF fill:#b3e6b3,stroke:#333,stroke-width:1px
    style RDFS fill:#b3e6b3,stroke:#333,stroke-width:1px
    style OWL fill:#b3e6b3,stroke:#333,stroke-width:1px
    style SHACL fill:#b3e6b3,stroke:#333,stroke-width:1px

    %% Level 3 - Tool nodes (lightest shades)
    style ERTools fill:#f2d9ff,stroke:#333,stroke-width:1px
    style UMLTools fill:#f2d9ff,stroke:#333,stroke-width:1px
    style TMFSID fill:#f2d9ff,stroke:#333,stroke-width:1px
    style GraphTools fill:#d9d9ff,stroke:#333,stroke-width:1px
    style SemanticTools fill:#d9f2d9,stroke:#333,stroke-width:1px
    style DocumentTools fill:#ffd9d9,stroke:#333,stroke-width:1px
    style Validation fill:#d9f2d9,stroke:#333,stroke-width:1px
```
