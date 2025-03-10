# On this page

- **This page serves as an introduction to the topic of SEMANTIC DATA MODELING.**
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
    style SDM fill:#ffcb6b,stroke:#2e7d32,stroke-width:2px
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
    click SHACL href "https://github.com/kanad13/data_modeling_techniques/34-shapes_constraint_language.md" "Click for more information"
```

# Semantic Data Modeling (RDF, RDFS, OWL, SHACL)

## Contextualize Semantic Data Modeling

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

    style SDM fill:#ffec5c,stroke:#555,stroke-width:2px
```

## Introduction to Semantic Data Modeling

- **Semantic Web Vision**
  - Aims for data with meaning and context, not just raw information.
  - Semantic web applications understand data meaning and relationships.
  - Can infer new knowledge from existing data.
  - In "Knowledge City" analogy: A city where information systems understand the meaning of everything.
- **Semantic Web Technologies**
  - Uses technologies like RDF, OWL, and SPARQL.
  - Employs ontologies (formal definitions of concepts and relationships).
  - Enables machines to process and understand data like humans.
- **Definition of Ontology**
  - Simple definition outside of computer science:
    - A formal representation of
      - knowledge as a set of concepts within a domain, and
      - the relationships between those concepts.
  - Notable ontologies outside of computer science:
    - "Periodic Table of Elements" - In this ontology
      - "Hydrogen" is a type of "Element".
      - Elements are types of "Matter".
    - "Vehicles" - In this ontology
      - "Car" is a type of "Vehicle".
      - "Truck" is a type of "Vehicle".
    - Here the relationships are
      - "is a type of"
      - "are types of"
- **Knowledge Graphs**
  - Knowledge graphs represent structured information using subject-predicate-object triples.
  - A subject (an entity) is linked to an object (another entity or a value) through a predicate (the relationship).
  - This format maps out how different pieces of data are interconnected.
  - Ontologies serve as blueprints in knowledge graphs, clarifying the types of entities involved (e.g., businesses, cuisines) and specifying relationships such as "is a type of" or "belongs to."
- **Example of a Search Engine**
  - Imagine a search engine enhanced with a knowledge graph.
  - When you query, "Show me restaurants in Paris that serve Italian food," the system:
    - Does not simply match keywords.
    - Recognizes "restaurants" as a type of business.
    - Understands "Italian food" as a specific category within cuisines.
    - Connects these entities through subject-predicate-object relationships in the graph.
  - This structured approach allows the search engine to efficiently filter and rank results, ensuring you receive options that precisely match your search criteria.
  - In this example, the knowledge graph uses an underlying ontology - a formal representation of various entities and their relationships - to define that:
    - "Restaurants" are a type of "Business."
    - "Italian food" is a subtype of "Cuisine."
- **Illustrative Example**
  - **Non-Semantic Approach**
    - System knows: "Rome" is a city in "Italy"; "Italy" is a country in "Europe".
    - Query: "What continent is Rome in?" - System cannot answer (relationship not understood).
  - **Semantic Approach**
    - Knowledge Graph: "Rome" `is in` "Italy" `is in` "Europe".
    - Query: "What continent is Rome in?" - System infers and answers "Europe".
    - Uses triples (subject-predicate-object) to represent relationships.
    - Enables inference based on defined relationships.
- **Evolution of Semantic Approach**
  - Semantic approach has evolved with increasing expressiveness.
  - Each stage adds more capabilities: RDF -> RDFS -> OWL.
  - Like building a "Knowledge City" in layers, starting from basic labeling (RDF) to complex knowledge representation (OWL).

```mermaid
graph TD
    SA[Semantic Approach Evolution]
    RDF[RDF: Basic Triples]
    RDFS[RDFS: Vocabulary & Classes]
    OWL[OWL: Complex Reasoning]

    SA --> RDF
    RDF --> RDFS
    RDFS --> OWL

    style SA fill:#ffec5c,stroke:#555,stroke-width:2px
    style RDF fill:#f9f,stroke:#333,stroke-width:1px
    style RDFS fill:#f9f,stroke:#333,stroke-width:1px
    style OWL fill:#f9f,stroke:#333,stroke-width:1px
```
