# On this page

- **This page serves as an introduction to the topic of RDFS - RDF SCHEMA.**
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
    style RDM fill:#ffebee,stroke:#d32f2f,stroke-width:2px
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
    style RDFS fill:#ffcb6b,stroke:#2e7d32,stroke-width:2px
    style OWL fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
    click ERTools href "https://github.com/kanad13/data_modeling/blob/master/120-data_modeling_tools/10-er_diagram_tools.md" "Click for more information"
    click UMLTools href "https://github.com/kanad13/data_modeling/blob/master/120-data_modeling_tools/20-uml_tools.md" "Click for more information"
    click TMFSID href "https://github.com/kanad13/data_modeling/blob/master/200-domain_specific_models/10-tm_forum.md" "Click for more information"
    click GraphTools href "https://github.com/kanad13/data_modeling/blob/master/120-data_modeling_tools/30-graph_data_modeling_tools.md" "Click for more information"
    click DocumentTools href "https://github.com/kanad13/data_modeling/blob/master/120-data_modeling_tools/50-json_based_modeling_tools.md" "Click for more information"
    click RDF href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/31-resource_description_framework.md" "Click for more information"
    click RDFS href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/32-resource_description_framework_schema.md" "Click for more information"
    click OWL href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/33-web_ontology_language.md" "Click for more information"

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
    click RDFSVocabulary href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/32-resource_description_framework_schema.md" "Click for more information"
    click SHACL href "https://github.com/kanad13/data_modeling/blob/master/100-data_modeling_techniques/34-shapes_constraint_language.md" "Click for more information"
```

# RDFS (RDF Schema)

## Contextualize RDFS

```mermaid
graph TD
    DM[Data Modeling Approaches]
    RDM[Relational Data Modeling]
    GDM[Graph Data Modeling]
    SDM[Semantic Data Modeling]

    DM --> RDM
    DM --> GDM
    DM --> SDM
    DM --> DDM[Document-oriented Data Modeling]

    SDM --> RDF[RDF - Resource Description  Framework]
    SDM --> RDFS[RDFS - RDF Schema]
    SDM --> OWL[OWL - Web Ontology  Language]
    SDM --> SHACL[SHACL - Shapes Constraint  Language]
    OWL --> SHACL
    SHACL --> Validation[Validation &  Data Quality]

    style RDFS fill:#ffec5c,stroke:#555,stroke-width:2px  %% Highlight RDFS Section
```

## Overview of RDFS

- **Introduction to RDFS:**
  - RDFS (RDF Schema) extends basic RDF model.
  - Provides vocabulary for describing classes, properties, and relationships.
  - Defines structure and semantics for RDF resources.
  - Think of RDFS as a simple type system for RDF.
  - RDFS is like providing `Grammar` to the `Vocabulary` of RDF.
- **Link Between RDF and RDFS:**
  - RDFS builds upon RDF to add structure and meaning.
  - RDF provides basic triples; RDFS provides rules for using them.
- **Analogy to language learning:**

| Component | Language Learning                       | Semantic Web                                        |
| --------- | --------------------------------------- | --------------------------------------------------- |
| **RDF**   | **Vocabulary** - words, basic sentences | Basic triple statements about resources             |
| **RDFS**  | **Grammar** - rules for word usage      | Rules for resource relationships and property usage |
| **OWL**   | **Syntax** - formal representation      | Advanced reasoning and relationships in ontology    |
| **SHACL** | **Constraints** - validation rules      | Ensures data quality and structure adherence        |

## RDFS Fixes The Shortcomings of RDF

### Basic RDF (Without RDFS)

```turtle
# RDF statements
:John :teaches :DatabaseCourse .
:Mary :attends :DatabaseCourse .
:DatabaseCourse :hasTitle "Database Systems" .
```

- This RDF data tells us some facts, but doesn't provide any semantic structure or constraints.
- We can't infer anything beyond what is explicitly stated.

### Enhanced with RDFS

```turtle
# Define classes
:Person rdf:type rdfs:Class .
:Student rdf:type rdfs:Class .
:Professor rdf:type rdfs:Class .
:Course rdf:type rdfs:Class .

# Define class hierarchy
:Student rdfs:subClassOf :Person .
:Professor rdfs:subClassOf :Person .

# Define properties and their domains/ranges
:teaches rdf:type rdf:Property .
:teaches rdfs:domain :Professor .
:teaches rdfs:range :Course .

:attends rdf:type rdf:Property .
:attends rdfs:domain :Student .
:attends rdfs:range :Course .

:hasTitle rdf:type rdf:Property .
:hasTitle rdfs:domain :Course .
:hasTitle rdfs:range rdfs:Literal .

# Instance data
:John rdf:type :Professor .
:Mary rdf:type :Student .
:DatabaseCourse rdf:type :Course .

:John :teaches :DatabaseCourse .
:Mary :attends :DatabaseCourse .
:DatabaseCourse :hasTitle "Database Systems" .
```

### Key Benefits of RDFS in This Example

- **Class Hierarchy:**
  - We can define that Students and Professors are subtypes of Persons.
- **Domain and Range Constraints:**
  - We can specify that:
    - Only Professors can teach Courses
    - Only Students can attend Courses
    - Only Courses can have titles
- **Inference Capabilities:**
  - With RDFS, we can infer new facts:
    - Since John teaches something, and only Professors can teach, John must be a Professor
    - Since Mary attends something, and only Students can attend, Mary must be a Student
    - Both John and Mary are automatically classified as Persons due to the subclass hierarchy
- **Semantic Validation:**
  - We can validate data against our schema.
  - For example, if we tried to state `:DatabaseCourse :teaches :John`, the RDFS processor would flag this as invalid because the domain of `:teaches` is `:Professor`, not `:Course`.

## RDFS in Action: E-commerce Example

- **Scenario:**
  - Defining basic vocabulary for e-commerce products and categories.
  - See below the RDFS Definitions using Turtle Syntax

```turtle
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .
@prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .
@prefix ex: <http://example.org/vocab#> .

# Classes
ex:Product a rdfs:Class ;
    rdfs:label "Product" ;
    rdfs:comment "An item offered for sale" .

ex:Category a rdfs:Class ;
    rdfs:label "Category" ;
    rdfs:comment "A grouping of related products" .

ex:ElectronicsCategory a rdfs:Class ;
    rdfs:subClassOf ex:Category ;
    rdfs:label "Electronics" ;
    rdfs:comment "Category for electronic devices" .

# Properties
ex:name a rdf:Property ;
    rdfs:label "Name" ;
    rdfs:domain ex:Product ;
    rdfs:range xsd:string ;
    rdfs:comment "The name of a product" .

ex:price a rdf:Property ;
    rdfs:label "Price" ;
    rdfs:domain ex:Product ;
    rdfs:range xsd:decimal ;
    rdfs:comment "The price of a product in currency units" .

ex:category a rdf:Property ;
    rdfs:label "Category" ;
    rdfs:domain ex:Product ;
    rdfs:range ex:Category ;
    rdfs:comment "The category to which a product belongs" .
```

- **Visual Representation of RDFS Example:**
  - This diagram visually represents the RDFS example from above.
  - It shows
    - `ex:Product`, `ex:Category`, and `ex:ElectronicsCategory` as classes, and
    - `ex:name`, `ex:price`, `ex:category` as properties.
  - Relationships like `rdfs:subClassOf`, `rdfs:domain`, and `rdfs:range` connect classes and properties, and define data types.

```mermaid
graph TD
    %% Classes
    Product(ex:Product <br> rdfs:Class)
    Category(ex:Category <br> rdfs:Class)
    ElectronicsCategory(ex:ElectronicsCategory <br> rdfs:Class)

    %% Properties as nodes
    name(ex:name <br> rdf:Property)
    price(ex:price <br> rdf:Property)
    category(ex:category <br> rdf:Property)

    %% Class relationships
    ElectronicsCategory -- rdfs:subClassOf --> Category

    %% Property domains and ranges
    Product -- rdfs:domain --> name
    name -- rdfs:range --> String(xsd:string)

    Product -- rdfs:domain --> price
    price -- rdfs:range --> Decimal(xsd:decimal)

    Product -- rdfs:domain --> category
    category -- rdfs:range --> Category

    %% Styling
    classDef classStyle fill:#f9f,stroke:#333,stroke-width:2px
    classDef propertyStyle fill:#ccf,stroke:#333,stroke-width:1px
    classDef datatypeStyle fill:#eee,stroke:#333,stroke-width:1px

    class Product,Category,ElectronicsCategory classStyle
    class name,price,category propertyStyle
    class String,Decimal datatypeStyle
```

## RDFS Vocabulary

- **Turtle (Terse RDF Triple Language):**
  - Concise, readable syntax for RDF.
  - Expresses RDF graphs in compact text format.
  - `@prefix`: Defines namespace shortcuts (e.g., `rdfs`, `rdf`, `ex`).
  - `a`: Shorthand for `rdf:type`.
  - Statements end with `.`.
  - `;`: Groups predicates for same subject.
  - `,`: Groups objects for same subject and predicate.
  - `xsd:decimal`, `xsd:string`: XML Schema datatypes for literals.
  - Indentation improves readability (not syntax-dependent).
- **Namespaces:**

  - `General Programming:`
    - Organize code elements, prevent naming conflicts (e.g., Java packages, Python modules).
  - `RDF/RDFS:`
    - Uniquely identify resources on the web using URIs. Prevent term collisions. Improve readability with prefixes.
  - **Example:**

    - In this example, namespace prefixes are foaf and ex.
    - The full URIs are defined at the beginning of the document.
    - And then in the remaining document, the prefixes are used to refer to the full URIs.
    - The `benefit of using namespace prefixes` is to reduce repetition and improve readability.
    - Instead of writing out full URIs each time, you can use these shorter prefixes to refer to your resources.

    ```turtle
    @prefix foaf: <http://xmlns.com/foaf/0.1/> .
    @prefix ex: <http://example.org/terms/> .

    ex:john a foaf:Person ;
        foaf:name "John Smith" ;
        ex:employeeID "E12345" .
    ```

- **Classes:**
  - `General Programming:`
    - Blueprints for objects
    - Encapsulate data and behavior
    - e.g., `Car`, `Person`
  - `RDF/RDFS:`
    - Categorize resources, define properties for class instances
    - e.g., `ex:Product`, `ex:Category`.
  - `Inheritance:`
    - `rdfs:subClassOf` for class inheritance
    - e.g., `ex:ElectronicsCategory` subclass of `ex:Category`.
- **Properties:**
  - `General Programming:`
    - Attributes or fields of a class (e.g., `color`, `size`).
  - `RDF/RDFS:`
    - Describe relationships between resources, define values they can have (e.g., `ex:name`, `ex:price`, `ex:category`).
  - `Example:`
    - `ex:name` property for product name, `ex:price` for product price.
- **Domains and Ranges:**
  - `General Programming:`
    - Check [here](https://www.mathsisfun.com/sets/domain-range-codomain.html)
  - `RDF/RDFS:`
    - `rdfs:domain` specifies class property applies to (subject).
    - `rdfs:range` specifies value/class of property (object).
    - Enforce data integrity and semantic meaning.
  - `Example:`
    - for `ex:name`
      - domain is `ex:Product`
      - range is `xsd:string`.
- **Labels and Comments:**
  - `General Programming:`
    - Human-readable names, explanations for code.
  - `RDF/RDFS:`
    - `rdfs:label` provides human-readable names for classes/properties.
    - `rdfs:comment` provides descriptions.
    - Improve human understanding of RDF/RDFS documents.
  - `Example:`
    - `rdfs:label "Product"` for `ex:Product` class,
    - `rdfs:comment "An item offered for sale"`.

Thank you for the feedback on the Mermaid diagram. I apologize for the continued issues. I have carefully reviewed your corrected diagram code and understand the necessary adjustments. I will ensure all future diagrams adhere to these guidelines.

Here is the updated overview diagram highlighting the **OWL** section, followed by the content for the **"OWL (Web Ontology Language)"** subsection:

```mermaid
graph TD
    DM[Data Modeling Approaches]
    RDM[Relational Data Modeling]
    GDM[Graph Data Modeling]
    SDM[Semantic Data Modeling]

    DM --> RDM
    DM --> GDM
    DM --> SDM
    DM --> DDM[Document-oriented Data Modeling]

    SDM --> RDF[RDF - Resource Description  Framework]
    SDM --> RDFS[RDFS - RDF Schema]
    SDM --> OWL[OWL - Web Ontology  Language]
    SDM --> SHACL[SHACL - Shapes Constraint  Language]
    OWL --> SHACL
    SHACL --> Validation[Validation &  Data Quality]

    style OWL fill:#ffec5c,stroke:#555,stroke-width:2px  %% Highlight OWL Section
```
