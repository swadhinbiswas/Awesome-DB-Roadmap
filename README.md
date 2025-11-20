# The 2026 Database Engineering Roadmap

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![GitHub stars](https://img.shields.io/github/stars/swadhinbiswas/jobprep.svg?style=social&label=Star)](https://github.com/swadhinbiswas/jobprep)

An industry-grade, comprehensive roadmap for anyone looking to master database engineering in 2026. This guide is designed for beginners and experienced developers who want to understand everything from fundamental concepts to modern, distributed database systems.

Whether you're aiming for a career in backend engineering, data engineering, or as a database administrator (DBA), this roadmap provides a structured learning path to help you succeed.

---

## Why This Roadmap?

*   **Comprehensive & Structured:** We cover everything from the ground up. No black boxes. The roadmap is organized logically, from fundamentals to advanced, specialized topics.
*   **Industry-Focused:** This isn't just a list of topics. It's a curated guide to the skills and technologies that are in demand in the industry today.
*   **From Theory to Practice:** We bridge the gap between theoretical knowledge and real-world application with practical project ideas.
*   **Community-Driven:** This roadmap is an open-source project. We encourage contributions to keep it the most up-to-date and relevant resource for database engineering.

---

## The Roadmap

This roadmap is divided into 8 key sections. While you can jump to any topic that interests you, we recommend following the sections in order for a more structured learning experience.

### 1. Fundamentals
The building blocks of every database system.
-   [ACID Properties](01%20-%20Fundamentals/ACID.md)
-   [CAP Theorem](01%20-%20Fundamentals/CAP%20Theorem.md)
-   [Indexes and Query Optimization](01%20-%20Fundamentals/Indexes.md)
-   [Transactions & Concurrency Control](01%20-%20Fundamentals/Transactions%20&%20Isolation.md)
-   [Replication & Sharding](01%20-%20Fundamentals/Replication.md)
-   [Storage Engines (WAL, MVCC)](01%20-%20Fundamentals/Storage%20Engines.md)
-   [Caching](01%20-%20Fundamentals/Caching.md)

### 2. Relational Databases (RDBMS)
The foundation of most applications. Master SQL and the most popular relational databases.
-   [SQL](02%20-%20RDBMS/Concepts.md)
-   [PostgreSQL](02%20-%20RDBMS/PostgreSQL.md)
-   [MySQL](02%20-%20RDBMS/MySQL.md)
-   [SQLite](02%20-%20RDBMS/SQLite.md)

### 3. NoSQL Databases
Explore the world beyond relational databases and understand when to use them.
-   [Key-Value Stores](03%20-%20NoSQL/Key-Value%20Stores.md) (e.g., Redis)
-   [Document Stores](03%20-%20NoSQL/Document%20Stores.md) (e.g., MongoDB)
-   [Wide-Column Stores](03%20-%20NoSQL/Wide-Column%20Stores.md) (e.g., Cassandra)
-   [Graph Databases](03%20-%20NoSQL/Graph%20Databases.md) (e.g., Neo4j)
-   [Vector Databases](03%20-%20NoSQL/Vector%20Databases.md) (e.g., Pinecone, Milvus)
-   [Search Engines](03%20-%20NoSQL/Search%20Engines.md) (e.g., Elasticsearch)

### 4. Data Modeling
Learn how to design efficient, scalable, and maintainable database schemas.
-   [ER Modeling](07%20-%20Data%20Modeling/ER%20Modeling.md)
-   [Star & Snowflake Schema](07%20-%20Data%20Modeling/Snowflake%20Schema.md)
-   [CQRS & Event Sourcing](07%20-%20Data%20Modeling/CQRS.md)
-   [Polyglot Persistence](07%20-%20Data%20Modeling/Polyglot%20Persistence.md)

### 5. Big Data & Analytics
Scale your knowledge to handle massive datasets.
-   [Data Warehouses](04%20-%20Big%20Data/Data%20Warehouses.md) (e.g., Snowflake, BigQuery)
-   [Distributed Storage](04%20-%20Big%20Data/Distributed%20Storage.md) (e.g., HDFS)
-   [Streaming Systems](04%20-%20Big%20Data/Streaming%20Systems.md) (e.g., Kafka, Flink)
-   [Query Engines](04%20-%20Big%20Data/Query%20Engines.md) (e.g., Presto, Trino)

### 6. Cloud Databases
Leverage the power of the cloud with managed database services.
-   [AWS (RDS, DynamoDB, Aurora)](05%20-%20Cloud%20Databases/AWS.md)
-   [Google Cloud (Cloud SQL, Spanner)](05%20-%20Cloud%20Databases/GCP.md)
-   [Azure (Cosmos DB, Azure SQL)](05%20-%20Cloud%20Databases/Azure.md)

### 7. Database Internals
Go deep and understand how databases *really* work.
-   [B-Trees vs. LSM Trees](06%20-%20Internals/B-Tree%20vs%20LSM.md)
-   [Query Planners & Optimizers](06%20-%20Internals/Query%20Planner.md)
-   [Consensus Algorithms (Paxos, Raft)](06%20-%20Internals/Raft%20Consensus.md)
-   [2PC & 3PC](06%20-%20Internals/2PC%20&%203PC.md)

### 8. Modern Databases
Explore the next generation of distributed SQL databases.
-   [Google Spanner](08%20-%20Modern%20Databases/Google%20Spanner.md)
-   [CockroachDB](08%20-%20Modern%20Databases/CockroachDB.md)
-   [TiDB](08%20-%20Modern%20Databases/TiDB.md)
-   [YugabyteDB](08%20-%20Modern%20Databases/YugabyteDB.md)

---

## How to Use This Roadmap

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/swadhinbiswas/jobprep.git
    ```
2.  **Explore the sections:** Start with the fundamentals and work your way through the topics. Each file contains key concepts, resources, and things to learn.
3.  **Track your progress:** The notes are in Markdown, so you can edit them and add checkboxes to track your learning.
4.  **Build the projects:** The best way to learn is by doing. Check out the `Practice Projects.md` file for ideas to apply your knowledge.

**Tip for Obsidian Users:** This repository is also a pre-built Obsidian vault. Just open the `Database Roadmap` folder as a vault in Obsidian to get features like graph view, wikilinks, and more.

---

## Contributing

This is a community-driven project, and we welcome contributions! If you see something missing, a topic that could be improved, or a new database that should be on the roadmap, please open an issue or submit a pull request.

Check out our contribution guidelines for more information (coming soon).

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.