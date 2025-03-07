# Document Databases & JSON-based Modeling

## Core Concepts

- **Introduction to Document Databases:**
  - Store data as documents (e.g., JSON, BSON).
  - Documents are collections of key-value pairs.
  - Schema-less or schema-flexible.
  - Well-suited for hierarchical data.
  - In "Flexible Neighborhoods" analogy: Like having varied building layouts within guidelines.
- **Documents:**
  - Represent entities or objects.
  - Business context examples: Customer profiles, product catalogs, blog posts.
  - Can have nested structures.
  - In "Flexible Neighborhoods" analogy: Documents are like `Buildings with varied layouts`.
- **Collections:**
  - Groups of related documents.
  - Similar to tables in relational databases.
  - Example: `Customers` collection, `Products` collection.
  - In "Flexible Neighborhoods" analogy: Collections are like `Neighborhoods with similar building types`.
- **Schema Flexibility:**
  - No fixed schema, documents can vary in structure.
  - Allows for easy evolution of data models.
  - In "Flexible Neighborhoods" analogy: Buildings can be modified without strict zoning laws.
- **Indexes:**
  - Improve query performance.
  - Can be created on fields within documents.
  - Example: Index on `email` field in `Customers` collection.
  - In "Flexible Neighborhoods" analogy: Indexes are like `Roads improving access to buildings`.

## Key Difference between Document and Relational Models

- **Schema Flexibility:**
  - `Document model`: No fixed schema, flexible document structures.
  - `Relational model`: Fixed schema, predefined table structures.
  - `In "Flexible Neighborhoods"`: Buildings can vary in layout, unlike fixed grid layouts.
- **Nested Data:**
  - `Document model`: Supports nested data structures.
  - `Relational model`: Requires normalization to handle nested data.
  - `In "Flexible Neighborhoods"`: Buildings can have varied internal layouts, unlike uniform building designs.
- **Data Retrieval:**
  - `Document model`: Retrieves entire documents.
  - `Relational model`: Retrieves rows and columns.
  - `In "Flexible Neighborhoods"`: Accessing a building vs. accessing specific rooms in a building.
- **Scalability:**
  - `Document model`: Horizontally scalable.
  - `Relational model`: Typically vertically scalable.
  - `In "Flexible Neighborhoods"`: Expanding neighborhoods vs. expanding individual buildings.

## Example: Modeling a Product Catalog using JSON

- **Scenario:**
  - Representing products in an e-commerce catalog.
- **Modeling Choices:**
  - **Documents:**
    - Represent products (`Product`).
  - **Fields:**
    - Store details like product name, description, price, category, and specifications.
  - **Nested Structures:**
    - Use nested objects for specifications and categories.
  - **Collections:**
    - Group products into a `Products` collection.
- **JSON Document Example:**
  - This example models a product catalog using JSON.
  - Each product is represented as a document with fields for product details and nested objects for specifications and categories.

```json
{
  "productID": "P001",
  "productName": "Smartphone X",
  "description": "Latest model with advanced features",
  "price": 799.99,
  "category": {
    "categoryID": "C001",
    "categoryName": "Electronics"
  },
  "specifications": {
    "screenSize": "6.5 inches",
    "batteryLife": "24 hours",
    "storage": "128GB",
    "camera": "12MP"
  }
}
```

## Example: Modeling a Blog Platform using JSON

- **Scenario:**
  - Representing blog posts and comments in a blogging platform.
- **Modeling Choices:**
  - **Documents:**
    - Represent blog posts (`Post`) and comments (`Comment`).
  - **Fields:**
    - Store details like post title, content, author, date, and comments.
  - **Nested Structures:**
    - Use nested objects for comments within posts.
  - **Collections:**
    - Group posts into a `Posts` collection.
- **JSON Document Example:**
  - This example models a blog platform using JSON.
  - Each post is represented as a document with fields for post details and nested objects for comments.

```json
{
  "postID": "B001",
  "title": "Introduction to JSON",
  "content": "JSON (JavaScript Object Notation) is a lightweight data-interchange format...",
  "author": "John Doe",
  "date": "2023-10-26",
  "comments": [
    {
      "commentID": "C001",
      "author": "Jane Smith",
      "content": "Great article!",
      "date": "2023-10-27"
    },
    {
      "commentID": "C002",
      "author": "Alice Johnson",
      "content": "Very informative, thanks!",
      "date": "2023-10-28"
    }
  ]
}
```
