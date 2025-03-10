# On this page

- **This page serves as an introduction to the topic of RELATIONAL DATA MODELING.**
- To check out other related topics, click on the links from the diagram below.
- To continue with the current topic, scroll down to read more.

```mermaid
graph LR
    %% Main node
    DM["Data Modeling Approaches"]
    style DM fill:#e5e5e5,stroke:#333,stroke-width:2px
    click DM href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/05-overview_of_data_modeling_concepts.md" "Click for more information"

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
    style RDM fill:#ffcb6b,stroke:#d32f2f,stroke-width:2px
    style GDM fill:#e3f2fd,stroke:#1565c0,stroke-width:2px
    style SDM fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    style DDM fill:#f3e5f5,stroke:#6a1b9a,stroke-width:2px
    click RDM href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/10-relational_data_modeling.md" "Click for more information"
    click GDM href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/20-graph_data_modeling.md" "Click for more information"
    click SDM href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/30-semantic_data_modeling.md" "Click for more information"
    click DDM href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/40-json_based_modeling.md" "Click for more information"

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
    click Tables href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/10-relational_data_modeling.md" "Click for more information"
    click NodesEdges href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/20-graph_data_modeling.md" "Click for more information"
    click Documents href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/40-json_based_modeling.md" "Click for more information"

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
    click RDF href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/31-resource_description_framework.md" "Click for more information"
    click RDFS href "https://github.com/kanad13/data_modeling_techniques/32-resource_description_framework_schema.md" "Click for more information"
    click OWL href "https://github.com/kanad13/data_modeling_techniques/33-web_ontology_language.md" "Click for more information"

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
    click Triples href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/31-resource_description_framework.md" "Click for more information"
    click RDFSVocabulary href "https://github.com/kanad13/data_modeling/techniques/32-resource_description_framework_schema.md" "Click for more information"
    click SHACL href "https://github.com/kanad13/data_modeling_techniques/34-shapes_constraint_language.md" "Click for more information"
```

# Relational Data Modeling

## Core Concepts of Relational Data Modeling

- **Introduction to Relational Model**
  - Widely used data modeling approach.
  - Organizes data into relations (tables).
  - Tables have columns (attributes) and rows (records).
  - Relationships established via shared attributes and keys.
- **Entities, Attributes, and Relationships**
  - `Entity:`
    - Real-world object or concept (e.g., Customer, Product).
    - Represented as a table.
    - In "Grid City" analogy: Entities are like _Buildings_.
  - `Attribute:`
    - Property or characteristic of an entity (e.g., Customer Name, Product Price).
    - Represented as a column in a table.
    - In "Grid City" analogy: Attributes are like _Building Features_ (e.g., number of floors, address).
  - `Relationship:`
    - Association between entities (e.g., Customer places Order).
    - Represented using foreign keys.
    - In "Grid City" analogy: Relationships are like _Roads connecting Buildings_.
- **Primary Keys and Foreign Keys**
  - `Primary Key (PK):`
    - Unique identifier for each row in a table.
    - Ensures each record is uniquely identifiable.
    - Example: `CustomerID` in `Customer` table.
    - Like a unique _Building Address_ in "Grid City".
  - `Foreign Key (FK):`
    - Attribute in one table referencing the primary key of another.
    - Establishes links between tables.
    - Example: `OrderID` table with `CustomerID` as FK referencing `Customer` table.
    - Like using a _Building Address_ in a separate registry to link back to the original building in "Grid City".

## Entity-Relationship (ER) Diagrams

- **What are ER Diagrams?**
  - Visual tools for relational data models.
  - Use symbols for entities, attributes, and relationships.
  - Simplify communication about database structure.
  - Like simplified _City Maps_ showing key buildings and roads.
- **ER Diagram Components:**
  - `Entities:`
    - Represented as rectangles.
    - In diagrams: `CUSTOMER`, `ORDER`.
    - Like _Building symbols_ on a city map.
  - **Attributes:**
    - Represented as ovals connected to entities.
    - In diagrams: `CustomerName`, `OrderID`.
    - Like _Labels for Building features_ on a map.
  - **Relationships:**
    - Represented as diamonds connecting entities.
    - In diagrams: `places`, `contains`.
    - Like _Road symbols_ connecting buildings on a map.
  - **Lines:**
    - Indicate relationship type (one-to-one, one-to-many, many-to-many).
    - Indicate _Road types_ (one-way, two-way, highways) on a map in terms of connection capacity.
    - Indicate _Connection capacity_ among the nodes.
- **Mermaid Syntax for ER Diagrams:**
  - Simple text-based syntax for creating diagrams.
  - Defines entities and relationships with specific notations.
  - Allows for clear, code-driven diagram creation.
  - Like a _City Map Key_ explaining symbols used.
- **Example ER Diagram Syntax Overview**
  - This diagram illustrates a basic ER diagram syntax using Mermaid.
  - It shows entities like `CUSTOMER`, `ORDER`, and `ORDER_ITEM` with their attributes, primary keys (PK), and foreign keys (FK).
  - Relationship cardinalities are also visualized (e.g., `||--o{` for one-to-many).
  - Comments (`%%`) explain key elements of the syntax.

```mermaid
%% Example Mermaid ER Diagram Syntax Overview
erDiagram
    %% One Customer (||) can place many Orders (o{)
    CUSTOMER ||--o{ ORDER : places
    %% Many Order Items (}o) belong to One Order (||)
    ORDER_ITEM }o--|| ORDER : contains

    CUSTOMER {
        int customerID PK "Primary Key for Customer"
        string customerName
        string address
        string phone
    }
    ORDER {
        int orderID PK "Primary Key for Order"
        date orderDate
        decimal totalAmount
        int customerID FK "Foreign Key referencing Customer"
    }
    ORDER_ITEM {
        int orderItemID PK "Primary Key for Order Item"
        int orderID FK "Foreign Key referencing Order"
        int productID FK "Foreign Key referencing Product (not shown)"
        int quantity
        decimal price
    }
```

- **Example: Modeling Customers and Orders**
  - **Scenario:**
    - E-commerce system needing to model customers and their orders.
  - **Entities:**
    - `Customer`: Represents individuals placing orders.
    - `Order`: Represents transactions made by customers.
  - **Suggested Attributes:**
    - **Customer Entity:**
      - `CustomerID` (PK): Unique identifier for each customer.
      - `CustomerName`: Name of the customer.
      - `Address`: Customer's address.
      - `Phone`: Customer's phone number.
    - **Order Entity:**
      - `OrderID` (PK): Unique identifier for each order.
      - `OrderDate`: Date when the order was placed.
      - `TotalAmount`: Total value of the order.
      - `CustomerID` (FK): Links to the `Customer` who placed the order.
  - **Relationship:**
    - "Customer places Order": One-to-many relationship.
      - One customer can place multiple orders.
      - Each order is placed by exactly one customer.
      - In "Grid City": One `Resident` (Customer) can be associated with multiple `Service Requests` (Orders).
  - **Mermaid ER Diagram:**
    - This diagram visually represents the `CUSTOMER` and `ORDER` entities and their one-to-many relationship ("places").
    - Entity attributes, primary keys (PK), and the foreign key (FK) are clearly outlined.
    - Comments (`%%`) within the diagram explain the cardinality notation (`||--o{`) for better understanding.

```mermaid
erDiagram
    %% Customer places Order - One-to-many
    CUSTOMER ||--o{ ORDER : places

    CUSTOMER {
        int customerID PK "Primary Key"
        string customerName
        string address
        string phone
    }
    ORDER {
        int orderID PK "Primary Key"
        date orderDate
        decimal totalAmount
        int customerID FK "Foreign Key"
    }
    %% Cardinality Explanation:
    %% || - one (exactly one)
    %% o{ - many (zero or more)
    %% Therefore, ||--o{ means: One CUSTOMER can be related to zero or more ORDERs.
    %% and each ORDER is related to exactly one CUSTOMER (implied by FK)
```
