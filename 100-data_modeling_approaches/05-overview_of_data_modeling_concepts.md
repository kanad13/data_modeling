# Introduction to Data Modeling

## Lego Blocks Analogy

- **Think of data modeling like building with LEGO blocks.**
  - Let's imagine you're building with LEGOs.
  - You don't just randomly throw bricks together and hope for the best. You usually have an idea in mind - maybe a house, a car, or a spaceship.
  - You plan out the different parts, how they connect, and what each part will be.
- **Data modeling is very similar**
  - But instead of LEGO bricks, we're working with `data` and building `digital systems` like databases, applications, or reports.
  - In simple terms, data modeling is the process of creating a blueprint for how data will be organized and structured within a system.
- **Data Modeling is about figuring out**
  - `What pieces (entities)` we need to build our system.
  - `What details (attributes)` each piece should have.
  - `How these pieces fit together (relationships)` to create a complete picture.
- **Importance of Data Modeling**
  - Just like a good LEGO plan makes building easier and results in a stronger, more functional creation, good data modeling makes building digital systems:
    - `Clearer:` Everyone understands the data and how it fits together.
    - `More Efficient:` Databases are designed logically, making them faster and easier to use.
    - `Less Error-prone:` By defining rules upfront, we reduce data inconsistencies and mistakes.
    - `Adaptable:` Well-modeled data is easier to change and update as needs evolve.

## Practical Example - Online Blog

- **Scenario:**
  - Imagine you're building a blog website.
  - You need to organize and structure the data for your blog.
- **Entities (Things):** Identify the main "things" to store:
  - `Posts:` The blog articles themselves.
  - `Authors:` The people writing the posts.
  - `Categories:` The topics for the posts.
- **Attributes (Details):** We define key information for each:
  - `Post:` Title, Content, Publication Date, Author, Category.
  - `Author:` Name, Email.
  - `Category:` Name.
- **Relationships (Connections):** We define how they connect:
  - `Author _writes_ Posts:` One Author can write many Posts.
  - `Post _belongs to_ Categories:` One Post can be in multiple Categories.
  - `Category _contains_ Posts:` One Category can have many Posts.
- **Concise "Data Model" (Conceptual):**

```mermaid
graph LR
    A[Author] -->|writes| B(Post)
    B -->|belongs to| C(Category)
    style A fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#ccf,stroke:#333,stroke-width:2px
    style C fill:#ccf,stroke:#333,stroke-width:2px
```

# On this page

- **This page serves as an introduction to the topic of DATA MODELING APPROACHES.**
- To check out other related topics, click on the links from the diagram below.
- To continue with the current topic, scroll down to read more.

```mermaid
graph LR
    %% Main node
    DM["Data Modeling Approaches"]
    style DM fill:#ffcb6b,stroke:#333,stroke-width:2px
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

## Abstraction Levels in Data Modeling

### Conceptual, Logical, and Physical Data Models

- Data Modeling is often done at three levels of abstraction:
  - **Conceptual:** High-level view of data, focusing on business needs.
  - **Logical:** More detailed, technology-independent view of data.
  - **Physical:** Database-specific view, considering implementation details.
- Each level serves a different purpose and audience:
  - **Conceptual:** Business stakeholders, project managers, data analysts.
  - **Logical:** Data modelers, database designers, developers.
  - **Physical:** Database administrators (DBAs), database developers.
- **Analogy:** Building a house
  - **Conceptual:** "I need a house with bedrooms, a kitchen, and a living room."
  - **Logical:** "The bedrooms will have beds and closets, the kitchen will have a stove and sink."
  - **Physical:** "The walls will be brick, the roof will be tile, the doors will be oak."

### Examples of Conceptual, Logical, and Physical Data Models

#### Understanding Conceptual Model through an Example

- Let's say we want to build a database for an online store.
- At the conceptual level, we might identify these key "things":
  - `Customer:` We need to store information about our customers.
  - `Product:` We sell products, so we need to track products.
  - `Order:` Customers place orders, so we need to manage orders.
- And the main relationships might be:
  - Customers _place_ Orders.
  - Orders _contain_ Products.
- This abstraction level
  - This is a very high-level view, focusing on the main entities and their relationships.
  - We are not concerned about how we will store this data or what technology we will use.
  - We are just trying to understand the business needs.
- Diagram below
  - We use simple boxes to represent our "things" (Customer, Order, Product).
  - Arrows show the relationships (Customers place Orders, Orders contain Products).
  - This is very basic – no details about what _kind_ of information we store about customers or products.

```mermaid
graph LR
    A[Customer] --> B(Order)
    B --> C(Product)
    style A fill:#f9f,stroke:#333,stroke-width:2px
    style B fill:#ccf,stroke:#333,stroke-width:2px
    style C fill:#ccf,stroke:#333,stroke-width:2px
```

#### Understanding Logical Model through an Example

- **Think of it as:**
  - A more detailed floor plan of your house.
  - Now you're thinking about _what's in each room_ - like bedrooms need beds, kitchens need stoves.
  - You're also thinking about _how rooms are connected_ more specifically.
- **Example: Online Store (Logical)**
  - Now we add more detail to our online store example.
  - We still don't care about _how_ this will be implemented in a database.

```mermaid
erDiagram
    CUSTOMER {
        int CustomerID PK
        string Name
        string Address
        string Email
        string PhoneNumber
    }
    PRODUCT {
        int ProductID PK
        string ProductName
        string Description
        decimal Price
        string Category
    }
    ORDER {
        int OrderID PK
        date OrderDate
        int CustomerID FK
        decimal TotalAmount
    }
    CUSTOMER ||--o{ ORDER : places
    ORDER ||--|{ PRODUCT : contains
```

- **Focus:**
  - We are now thinking about _what information_ we need to store about each entity.
  - For example, for a customer, we might want to store their name, address, email, and phone number.
  - For a product, we might want to store its name, description, price, and category.
  - We also define the relationships more clearly:
    - A customer can place many orders (one-to-many).
    - An order can contain many products (many-to-many).

#### Understanding Physical Model through an Example

- **Think of it as:**
  - The blueprints for your house, ready for construction.
- **Focus:**
  - Database-specific.
  - Now we consider the _specific database system_ we'll use (like MySQL, PostgreSQL, SQL Server, etc.).
  - We choose _data types_ that are supported by that database.
  - We think about _performance_ – indexes, storage, etc.
  - We create actual _tables_, _columns_, and define _constraints_ (rules) to ensure data quality.
- **Example of SQL DDL (for PostgreSQL):**

```sql
CREATE TABLE customers (
    customer_id INT PRIMARY KEY,
    name VARCHAR(255),
    address TEXT,
    email VARCHAR(100) UNIQUE,
    phone_number VARCHAR(20)
);

CREATE TABLE products (
    product_id INT PRIMARY KEY,
    product_name VARCHAR(255),
    description TEXT,
    price DECIMAL(10, 2),
    category VARCHAR(50)
);

CREATE TABLE orders (
    order_id INT PRIMARY KEY,
    order_date DATE,
    customer_id INT REFERENCES customers(customer_id),
    total_amount DECIMAL(12, 2)
);
```

## Overview of Main Data Modeling Approaches

- **Relational Data Modeling:**
  - `Structure:` Tables with rows and columns
  - `Relationships:` Defined through keys
  - `Analogy:` "Grid City" - well-defined blocks, streets
  - `Best for:` Structured data, transactions
- **Graph Data Modeling:**
  - `Structure:` Nodes (entities) and edges (relationships)
  - `Focus:` Connections and networks
  - `Analogy:` "Network City" - connections are key
  - `Best for:` Relationship-rich data, network analysis
- **Semantic Data Modeling:**
  - `Structure:` Triples (subject-predicate-object)
  - `Focus:` Meaning, context, knowledge
  - `Analogy:` "Knowledge City" - semantically labeled elements
  - `Best for:` Knowledge graphs, data integration, reasoning
- **Document-oriented Data Modeling:**
  - `Structure:` Flexible JSON documents
  - `Focus:` Flexibility, schema-on-read
  - `Analogy:` "Flexible Neighborhoods" - varied layouts within guidelines
  - `Best for:` Content management, catalogs, evolving data

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

    style DM fill:#ffec5c,stroke:#555,stroke-width:2px
    style RDM fill:#f9f,stroke:#333,stroke-width:1px
    style GDM fill:#ccf,stroke:#333,stroke-width:1px
    style SDM fill:#cfc,stroke:#333,stroke-width:1px
    style DDM fill:#fcc,stroke:#333,stroke-width:1px

    classDef approachStyle fill:#eee,stroke:#333,stroke-width:1px
    class RDM,GDM,SDM,DDM approachStyle
```
