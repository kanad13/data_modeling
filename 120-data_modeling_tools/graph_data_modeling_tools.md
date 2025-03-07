# Graph Database Tools (For Graph Data Models)

- **What are they?**
  - Tools designed for visualizing and working with graph data models.
  - Often specific to graph databases or general graph visualization.
- **What do they help with?**
  - Exploring relationships between data points (nodes and edges).
  - Designing graph database schemas visually.
  - Querying and analyzing graph data.
- **Example Tools:**
  - [Neo4j Bloom](https://neo4j.com/product/bloom/)
  - [Gephi](https://gephi.org)

```mermaid
graph LR
    Person1(Person) --> FRIEND_OF -- since 2020 --> Person2(Person)
    Person1 --> CREATED --> Post1(Post)
    Post1 --> LIKED -- by --> Person2
    style Person1 fill:#f9f,stroke:#333,stroke-width:2px
    style Person2 fill:#f9f,stroke:#333,stroke-width:2px
    style Post1 fill:#ccf,stroke:#333,stroke-width:2px
```
