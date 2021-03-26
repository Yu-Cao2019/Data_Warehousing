## Graph Databases

### What is a Graph
Graph is a bastract, mathematical representation of two or more entities, showing relations between objects.

It made up of two components -- the nodes and the edges.

### What is a Graph Databases
Graph database is used to model data in a form of graph. It stores data using nodes, relationships and properties.

### Advantage of Graph Databases
- In RDBMS, performance suffers as the number and depth of relationships increases. 
However, in graph databases, performance remains high even if the amount of data grws significantly.
- Graph databases are schema-free, making them can add nodes, labels, subgraphs at any point.
- Graph databases are agility. They envolve data model with the rest of application.

### Comparing Graph Databases vs. RDBMS
|Graph Database|RDBMS|
|--------------|-----|
|Data is stored in graphs|Data is stored in tables|
|Nodes|Rows|
|Properties and their values|Columns and data|
|Connected nodes are defined by relationships|Constraints are used for relationships|
|Database traversal|Table joins|

### Two Main Properties of Graph Databases
- Some graoh databases use 'native' graph storage specifically designed to store and manage graphs and others use relational or object-oriented databases. (Neo4j is a native graph database that is structured for native graph storage)
- Graph databases are index-free adjacency, indicating that native graph processing is the most efficient way to process data. The connected nodes point to each other in the database.

#### Native vs. Non-Native
Non-native graph is persistence layer and the data will grow. It need more hardware to solve the problem, and lower latencies for larger graphs. Native graph has scaling advantage and it store, query and traverse large interconnected datasets in real-time.

### Graph Databases Terminology
- Vertex/Node: an entity marked with a unique identifier analogous to primary key in a relational database.
- Edge: represents a relationship. Also known as a link or arc, an edge defines relationship between vertices or objects connecting vertices.
- Path: A set of vertices, along with the edges between those vertices. The vertices in a graph are all different from each other. If edges are directed, the path is a directed path. If the graph is undirected, the paths in it are undirected paths.
- Loop: Edge that connects vertex to itself.

#### Operations on Graphs
Insert, Read, Update, Delete data, Union of graphs, intersevtion of graphs, traversal of graph.

### When to Use Graph Databases
- Fraud detection: Fraudsters are using stolen identities to form fraud rings so graph database looks beyond individual data points to the actual connections that link them to see the patterns.
- Social networks: Socialrecommendations,Friend-of-Friendrecommendations.
- Identity and access management: Manage multiple changing roles, groups, products and access authorization and inheritances.
- Master data management: Master data, such as organizational and product data, has deep hierarchies with top-down, lateral and diagonal connections.
- Network and IT operations.

Don’t use graph databases for the first time on something mission-critical
Graph database like Neo4j is not a general purpose database. It works well with specific use cases such as where the relationship is as (or more) important as the entities that it connects.

## Neo4j

### What is Neo4j Database
Neo4j is a database used to stores information and find it later. It can be written in Java and optimized for dealing with graph data. It is labeled property graph.

Cypher is Neo4j’s query language which is similar to SQL, but optimized for graphs. And cypher is declarative language, which means it describes what you need, not how to get it.

Neo4j is transactional, ACID-compliant database and is made for online transaction processing.
Neo4j is released in 2007, sponsored by Neo4j, Inc. And it is designed to scale. It is an open-source and community and enterprise versions.

### The Features of Neo4j
- Intuitive: it uses a graph model for data representation.
- Reliable: It has full ACID transactions.
- Durable/Fast: it is custom disk-based, native storage engine.
- Massively scalable: its scale is up to several billion.
- Highly available: It is highly available when distributed across multiple machines.
- Expressive: It has graph query language.
- Fast: It has powerful traversal framework for high-speed graph queries.
- Embeddable: it is embeddable with a few small jar files.
- Simple: It is accessible by REST interface or an object-oriented Java API.

### Four Data Constructs
- Nodes: These are the main data elements that are interconnected through relationships. A node can have one or more labels (that describe its role) and properties (i.e. attributes).
- Relationships: A relationship connects two nodes that, in turn, can have multiple relationships. Relationships can have one or more properties. 
- Properties: These are attributes of both nodes and relationships. Neo4j allows for storing data as key-value pairs, which means properties can have any value (string, number, or Boolean) 
- Labels: These are used to group nodes, and each node can be assigned multiple labels. Labels are indexed to speed up finding nodes in a graph.


