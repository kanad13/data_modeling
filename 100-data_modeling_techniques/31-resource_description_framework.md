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
