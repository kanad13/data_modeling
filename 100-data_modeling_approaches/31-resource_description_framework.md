# On this page

- **This page serves as an introduction to the topic of RDF - RESOURCE DESCRIPTION FRAMEWORK.**
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
    style TMFSID fill:#ffebee,stroke:#d32f2f,stroke-width:2px
    style GraphTools fill:#e3f2fd,stroke:#1565c0,stroke-width:2px
    style DocumentTools fill:#f3e5f5,stroke:#6a1b9a,stroke-width:2px
    style RDF fill:#ffcb6b,stroke:#2e7d32,stroke-width:2px
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

# RDF (Resource Description Framework)

- **Introduction to RDF:**
  - RDF (Resource Description Framework) is a standard for data interchange on the Web.
  - Represents information as `triples`
    - Subject-Predicate-Object
  - Designed for machine readability and data integration.
  - Foundation of Semantic Web.
  - In "Knowledge City" analogy: RDF is like the `basic labeling system` for everything in the city.
- **RDF Triples: Subject, Predicate, Object:**
  - **Subject:**
    - Entity or resource being described.
    - "What" or "who" the statement is about.
    - Example: `Product:P456`.
  - **Predicate:**
    - Property or relationship describing the subject.
    - Connects subject to object.
    - Defines nature of relationship.
    - Example: `hasName`.
  - **Object:**
    - Value or entity related to subject via predicate.
    - Can be literal value or another resource.
    - Example: `"Laptop"` or `Category:Electronics`.
- **Example: Product Information in RDF:**
  - Representing product "P456" with name "Laptop", price 1200, category "Electronics".

```mermaid
graph LR
    %% Resources (Subjects and Objects)
    Product(Product:P456)
    Category(Category:Electronics)

    %% Properties (Predicates)
    Product-- hasName -->ProductName("Laptop")
    Product-- hasID -->ProductID("P456")
    Product-- hasPrice -->Price("1200"^^xsdinteger)
    Product-- belongsToCategory -->Category
    Category-- hasName -->CategoryName("Electronics")

    %% Styling for Resources and Literals
    style Product fill:#f9f,stroke:#333,stroke-width:2px
    style Category fill:#ccf,stroke:#333,stroke-width:2px
    classDef literal fill:#eee,stroke:#333,stroke-width:1px
    class ProductName,ProductID,Price,CategoryName literal

    %% Triple visual representation
    subgraph RDF_Triples
    direction TB
        T1["Product:P456 <br/> hasName <br/> 'Laptop'"]
        T2["Product:P456 <br/> hasID <br/> 'P456'"]
        T3["Product:P456 <br/> hasPrice <br/> '1200'^^xsdinteger"]
        T4["Product:P456 <br/> belongsToCategory <br/> Category:Electronics"]
        T5["Category:Electronics <br/> hasName <br/> 'Electronics'"]
    end

    ProductName --> T1
    ProductID --> T2
    Price --> T3
    Category --> T4
    CategoryName --> T5
    Product --> T1 & T2 & T3 & T4

    linkStyle 0,1,2,3,4,5,6,7,8,9,10 stroke:#999,stroke-width:1px,color:#555
```

- **Note on RDF Identifiers:**
  - Formal RDF uses URIs/IRIs (e.g., `http://example.org/product/P456`).
  - Examples use simplified identifiers (e.g., `Product:P456`) for readability.
  - In practice, these map to full URIs in namespaces.
  - Predicates like `hasName` also use full URIs in real systems.
