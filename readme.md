# Introduction to Data Modeling

## Overview of the Repository

This repository serves as an introduction to the topic of data modeling. It contains documents that provide insights into various data modeling techniques, tools, and industry standards.

## Purpose of Each Document

1. [100-data_modeling_techniques.md](./100-data_modeling_techniques.md)
   - **Purpose:** Introduces the concept of data modeling and delves into various techniques such as relational data modeling, graph data modeling, semantic data modeling (RDF, RDFS, OWL, SHACL), and Document Databases & JSON-based Modeling.
   - **Link:** [100-data_modeling_techniques.md](./100-data_modeling_techniques.md)

2. [120-data_modeling_tools.md](./120-data_modeling_tools.md)
   - **Purpose:** Provides an overview of various data modeling tools available for different types of data models.
   - **Link:** [120-data_modeling_tools.md](./120-data_modeling_tools.md)

3. [200-tm_forum.md](./200-tm_forum.md)
   - **Purpose:** Contains details about TM Forum's Information Framework components (SID, eTOM, and TAM), and how these components work together, about Open Digital Architecture (ODA) and TM Forum Open APIs.
   - **Link:** [200-tm_forum.md](./200-tm_forum.md)

## Navigation

```mermaid
graph LR
    DM[Data Modeling Approaches]
    RDM[Relational]
    GDM[Graph]
    SDM[Semantic]
    DDM[Document-oriented]

    DM --> RDM
    DM --> GDM
    DM --> SDM
    DM --> DDM

    RDM --> Tables[Tables & SQL]
    GDM --> NodesEdges[Nodes & Edges]
    SDM --> Triples[RDF Triples]
    DDM --> Documents[JSON Documents]

    Tables --> ERTools[ER Diagram Tools]
    Tables --> UMLTools[UML Tools]
    Tables --> TMFSID[TMForum SID]
    NodesEdges --> GraphTools[Graph Database Tools]
    Triples --> SemanticTools[Semantic Web Tools]
    Documents --> DocumentTools[Document DB Tools]

    style DM fill:#ffec5c,stroke:#555,stroke-width:2px
    style RDM fill:#f9f,stroke:#333,stroke-width:1px
    style GDM fill:#ccf,stroke:#333,stroke-width:1px
    style SDM fill:#cfc,stroke:#333,stroke-width:1px
    style DDM fill:#fcc,stroke:#333,stroke-width:1px

    classDef approachStyle fill:#eee,stroke:#333,stroke-width:1px
    class RDM,GDM,SDM,DDM approachStyle

    classDef toolStyle fill:#e1e1e1,stroke:#555,stroke-width:1px
    class ERTools,UMLTools,GraphTools,SemanticTools,DocumentTools,TMFSID toolStyle
```
