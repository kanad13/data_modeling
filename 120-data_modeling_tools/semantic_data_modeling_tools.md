# Semantic Data Modeling Tools

## What are they?

- Tools for creating and managing semantic data models (ontologies, RDF graphs).
- Support RDF, RDFS, OWL, and SHACL standards.

## What do they help with?

- Building ontologies (defining classes, properties, relationships semantically).
- Editing RDF data and schemas.
- Validating RDF data against SHACL shapes.
- Reasoning and inference with semantic data.

## Example Tools

- [Protégé](https://github.com/protegeproject/protege)
- [TopBraid Composer](https://topbraidcomposer.org/html/What_is_TopBraid_Composer.htm)

```mermaid
graph LR
    Product(ex:Product <br> rdfs:Class)
    Category(ex:Category <br> rdfs:Class)
    ElectronicsCategory(ex:ElectronicsCategory <br> rdfs:Class)
    ElectronicsCategory -- rdfs:subClassOf --> Category
    style Product fill:#f9f,stroke:#333,stroke-width:2px
    style Category fill:#ccf,stroke:#333,stroke-width:2px
    style ElectronicsCategory fill:#ccf,stroke:#333,stroke-width:2px
```
