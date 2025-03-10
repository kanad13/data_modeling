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
    style DM fill:#ffd60a,stroke:#333,stroke-width:2px

    %% First level connections
    DM --> RDM
    DM --> GDM
    DM --> SDM
    DM --> DDM

    %% Main approaches - Parent Level 1
    RDM[Relational Data Modeling]
    GDM[Graph Data Modeling]
    SDM[Semantic Data Modeling]
    DDM[Document-oriented Data Modeling]
    style RDM fill:#ccc5b9,stroke:#333,stroke-width:1px,color:#333
    style GDM fill:#fffcf2,stroke:#333,stroke-width:1px,color:#333
    style SDM fill:#e5e5e5,stroke:#333,stroke-width:1px,color:#333
    style DDM fill:#e1e5f2,stroke:#333,stroke-width:1px,color:#333

    %% First level Implementations - Parent Level 2
    Tables[Tables & SQL]
    NodesEdges[Nodes & Edges]
    Documents[JSON Documents]
    RDM --> Tables
    GDM --> NodesEdges
    DDM --> Documents
    style Tables fill:#e0dad5,stroke:#333,stroke-width:1px,color:#333
    style NodesEdges fill:#fffef9,stroke:#333,stroke-width:1px,color:#333
    style Documents fill:#f0f2f7,stroke:#333,stroke-width:1px,color:#333

    %% Tools and Technologies & Semantic specifics - Parent Level 3
    ERTools[ER Diagram Tools]
    UMLTools[UML Tools]
    TMFSID[TMForum SID]
    GraphTools[Graph Database Tools]
    DocumentTools[Document DB Tools]
    RDF[RDF - Resource Description Framework]
    RDFS[RDFS - RDF Schema]
    OWL[OWL - Web Ontology Language]
    Tables --> ERTools
    Tables --> UMLTools
    Tables --> TMFSID
    NodesEdges --> GraphTools
    Documents --> DocumentTools
    SDM --> RDF
    SDM --> RDFS
    SDM --> OWL
    style ERTools fill:#e8e4e1,stroke:#333,stroke-width:1px,color:#333
    style UMLTools fill:#e8e4e1,stroke:#333,stroke-width:1px,color:#333
    style TMFSID fill:#e8e4e1,stroke:#333,stroke-width:1px,color:#333
    style GraphTools fill:#fffdf6,stroke:#333,stroke-width:1px,color:#333
    style DocumentTools fill:#f9fafc,stroke:#333,stroke-width:1px,color:#333
    style RDF fill:#d4d4d4,stroke:#333,stroke-width:1px,color:#333
    style RDFS fill:#d4d4d4,stroke:#333,stroke-width:1px,color:#333
    style OWL fill:#d4d4d4,stroke:#333,stroke-width:1px,color:#333

    %% Semantic Data Modeling specifics - Deeper Level 4
    Triples[RDF Triples]
    SHACL[SHACL - Shapes Constraint Language]
    RDF --> Triples
    OWL --> SHACL
    style Triples fill:#c2c2c2,stroke:#333,stroke-width:1px,color:#333
    style SHACL fill:#c2c2c2,stroke:#333,stroke-width:1px,color:#333
```

## With Hyperlinks

```mermaid
graph LR
    %% Main node
    DM["Data Modeling Approaches"]
    style DM fill:#ffd60a,stroke:#333,stroke-width:2px
    click DM href "https://google.com" "Click for more information"

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
    style RDM fill:none,stroke:#e74c3c,stroke-width:2px
    style GDM fill:none,stroke:#3498db,stroke-width:2px
    style SDM fill:none,stroke:#2ecc71,stroke-width:2px
    style DDM fill:none,stroke:#9b59b6,stroke-width:2px
    click RDM href "https://google.com" "Click for more information"
    click GDM href "https://google.com" "Click for more information"
    click SDM href "https://google.com" "Click for more information"
    click DDM href "https://google.com" "Click for more information"

    %% First level Implementations - Parent Level 2
    Tables["Tables & SQL"]
    NodesEdges["Nodes & Edges"]
    Documents["JSON Documents"]
    RDM --> Tables
    GDM --> NodesEdges
    DDM --> Documents
    style Tables fill:none,stroke:#e74c3c,stroke-width:2px
    style NodesEdges fill:none,stroke:#3498db,stroke-width:2px
    style Documents fill:none,stroke:#9b59b6,stroke-width:2px
    click Tables href "https://google.com" "Click for more information"
    click NodesEdges href "https://google.com" "Click for more information"
    click Documents href "https://google.com" "Click for more information"

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
    style ERTools fill:none,stroke:#e74c3c,stroke-width:2px
    style UMLTools fill:none,stroke:#e74c3c,stroke-width:2px
    style TMFSID fill:none,stroke:#e74c3c,stroke-width:2px
    style GraphTools fill:none,stroke:#3498db,stroke-width:2px
    style DocumentTools fill:none,stroke:#9b59b6,stroke-width:2px
    style RDF fill:none,stroke:#2ecc71,stroke-width:2px
    style RDFS fill:none,stroke:#2ecc71,stroke-width:2px
    style OWL fill:none,stroke:#2ecc71,stroke-width:2px
    click ERTools href "https://google.com" "Click for more information"
    click UMLTools href "https://google.com" "Click for more information"
    click TMFSID href "https://google.com" "Click for more information"
    click GraphTools href "https://google.com" "Click for more information"
    click DocumentTools href "https://google.com" "Click for more information"
    click RDF href "https://google.com" "Click for more information"
    click RDFS href "https://google.com" "Click for more information"
    click OWL href "https://google.com" "Click for more information"

    %% Semantic Data Modeling specifics - Deeper Level 4
    Triples["RDF Triples"]
    SHACL["SHACL - Shapes Constraint Language"]
    RDF --> Triples
    OWL --> SHACL
    style Triples fill:none,stroke:#2ecc71,stroke-width:2px
    style SHACL fill:none,stroke:#2ecc71,stroke-width:2px
    click Triples href "https://google.com" "Click for more information"
    click SHACL href "https://google.com" "Click for more information"
```
