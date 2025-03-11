# On this page

- **This page serves as an introduction to the topic of GRAPH DATA MODELING.**
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
    style GDM fill:#ffcb6b,stroke:#1565c0,stroke-width:2px
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
    style RDF fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    style RDFS fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    style OWL fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    click ERTools href "https://github.com/kanad13/data_modeling/blob/master/120-data_modeling_tools/10-er_diagram_tools.md" "Click for more information"
    click UMLTools href "https://github.com/kanad13/data_modeling/blob/master/120-data_modeling_tools/20-uml_tools.md" "Click for more information"
    click TMFSID href "https://github.com/kanad13/data_modeling/blob/master/200-domain_specific_models/10-tm_forum.md" "Click for more information"
    click GraphTools href "https://github.com/kanad13/data_modeling/blob/master/120-data_modeling_tools/30-graph_data_modeling_tools.md" "Click for more information"
    click DocumentTools href "https://github.com/kanad13/data_modeling/blob/master/120-data_modeling_tools/50-json_based_modeling_tools.md" "Click for more information"
    click RDF href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_approaches/31-resource_description_framework.md" "Click for more information"
    click RDFS href "https://github.com/kanad13/data_modeling_techniques/32-resource_description_framework_schema.md" "Click for more information"
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
    click SHACL href "https://github.com/kanad13/data_modeling_techniques/34-shapes_constraint_language.md" "Click for more information"
```

# Graph Data Modeling (Property Graphs)

## Core Concepts

- **Introduction to Graph Data Modeling:**
  - Focuses on relationships between data points.
  - Represents data as networks of nodes and edges.
  - Nodes are entities, edges are relationships.
  - Well-suited for complex, interconnected data.
  - In "Network City" analogy: Like focusing on `Connections between Locations`.
- **Nodes (Vertices):**
  - Represent entities or objects.
  - Business context examples: Customers, products, categories.
  - Can have labels to categorize type.
  - In "Network City" analogy: Nodes are like `Key Locations` (e.g., landmarks, buildings, intersections).
- **Edges (Relationships):**
  - Represent connections between nodes.
  - Have direction and type.
  - Examples: "CUSTOMER -purchased-> PRODUCT", "PRODUCT -inCategory-> CATEGORY".
  - Can have labels to describe the relationship.
  - In "Network City" analogy: Edges are like `Roads or Transit Lines` connecting locations.
- **Properties:**
  - Key-value pairs describing nodes and edges.
  - Nodes: `'Customer' node with properties 'name: "Alice"', 'city: "London"'`.
  - Edges: `'purchased' edge with property 'date: "2023-10-26"'`.
  - Add detail and context to nodes and edges.
  - In "Network City" analogy: Properties are like `Attributes of Locations or Roads` (e.g., location name, road length, traffic capacity).
- **Labels:**
  - Categorization tags for nodes and edges.
  - Group nodes/edges by type.
  - Node labels: `'Customer'`, `'Product'`, `'Order'`.
  - Edge labels: `'purchased'`, `'locatedIn'`, `'employs'`.
  - Enable efficient filtering and querying.
  - In "Network City" analogy: Labels are like `Zone Types` (e.g., residential zone, commercial zone) or `Road Classifications` (highway, street).

## Key Difference between Graph and Relational Models

- **Explicit Relationships:**
  - `Graph model`: Relationships are primary, first-class entities.
  - `Relational model`: Relationships are implicit, through foreign keys.
  - `In "Network City"`: Roads (edges) are as important as Buildings (nodes).
- **No Foreign Keys:**
  - `Graph model`: Direct connections via edges, no need for foreign keys.
  - `Relational model`: Relies heavily on foreign keys to link tables.
  - `In "Network City"`: Direct roads, no need for address registries to find connections.
- **Properties on Nodes & Edges:**
  - `Graph model`: Nodes and edges can have properties.
  - `Relational model`: Properties are only on entities (tables).
  - `In "Network City"`: Both Locations and Roads have attributes (name, length, type).
- **Flexible Schema:**
  - `Graph model`: No fixed schema, nodes of same type can vary in properties.
  - `Relational model`: Strict, predefined schema for tables.
  - `In "Network City"`: Neighborhoods (node types) can evolve with varied building styles.
- **Query Focus:**
  - `Graph model`: Focus on traversing relationships.
  - `Relational model`: Focus on joining tables.
  - `In "Network City"`: Queries are about finding paths and connections, not just looking up locations in lists.

## Example: Modeling a Social Network using Property Graphs

- **Scenario:**
  - Representing connections and interactions in a social network.
- **Modeling Choices:**
  - **Nodes:**
    - Represent people (`Person`) and content (`Post`, `Interest`).
  - **Edges:**
    - Represent relationships (`FRIEND_OF`), actions (`CREATED`, `LIKED`, `SHARED`, `COMMENTED`), and interests (`INTERESTED_IN`).
  - **Properties:**
    - Store details like names, ages, locations for people; content, timestamps for posts; names for interests; and timestamps, comments for relationships.
  - **Labels:**
    - Use labels like `Person`, `Post`, `Interest`, `FRIEND_OF` to categorize nodes and edges.
- **Mermaid Graph Diagram:**
  - This diagram models a social network using a property graph.
  - Nodes represent `Person`, `Post`, and `Interest` entities with labels and properties.
  - Edges illustrate relationships like `FRIEND_OF`, `CREATED`, `LIKED`, etc., also with labels and properties.
  - Styling is used to visually differentiate node types.

```mermaid
graph LR
    %% Nodes with Labels and Properties
    P1(Person<br>name: 'Alice'<br>age: 28)
    P2(Person<br>name: 'Bob'<br>age: 32)
    P3(Person<br>name: 'Carol'<br>age: 25)
    P4(Person<br>name: 'David'<br>age: 40)

    Post1(Post<br>content: 'Great day!'<br>time: '10:30')
    Post2(Post<br>content: 'Check article'<br>time: '14:15')

    I1(Interest<br>name: 'Photography')
    I2(Interest<br>name: 'Hiking')
    I3(Interest<br>name: 'Technology')

    %% Edges with Labels and Properties
    P1 -- FRIEND_OF<br>since: '2020' --> P2
    P1 -- FRIEND_OF<br>since: '2019' --> P3
    P2 -- FRIEND_OF<br>since: '2021' --> P4

    P1 -- CREATED --> Post1
    P2 -- CREATED --> Post2

    P3 -- LIKED --> Post1
    P4 -- SHARED --> Post2
    P1 -- COMMENTED<br>text: 'Thanks!' --> Post1

    P1 -- INTERESTED_IN --> I1
    P1 -- INTERESTED_IN --> I3
    P2 -- INTERESTED_IN --> I2
    P3 -- INTERESTED_IN --> I1
    P4 -- INTERESTED_IN --> I2
    P4 -- INTERESTED_IN --> I3

    %% Styling for clarity
    classDef personNode fill:#f9f,stroke:#333,stroke-width:1px
    classDef postNode fill:#ccf,stroke:#333,stroke-width:1px
    classDef interestNode fill:#cfc,stroke:#333,stroke-width:1px
    class P1,P2,P3,P4 personNode
    class Post1,Post2 postNode
    class I1,I2,I3 interestNode
```
