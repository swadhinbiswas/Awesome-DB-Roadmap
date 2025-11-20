# 03 – NoSQL Ecosystem

NoSQL systems trade strict relational guarantees for **scalability, flexibility, or performance** in specific use cases.

---

## 📌 Overview

- [ ] Understand why NoSQL emerged
- [ ] Map use cases to the right NoSQL family
- [ ] Learn the strengths and weaknesses of each type

---

## 🧱 Families

### [[Key-Value Stores]]

- [ ] Understand **key → value** access patterns
- [ ] Typical use cases: caching, sessions, feature flags
- [ ] Learn about examples like Redis, DynamoDB (key-value aspect)

### [[Document Stores]]

- [ ] Store and query **JSON-like documents**
- [ ] Understand flexible schemas vs schema-on-write in RDBMS
- [ ] Learn use cases: content management, user profiles, catalogs

### [[Wide-Column Stores]]

- [ ] Understand **column families** and sparse storage
- [ ] Learn about Cassandra, HBase, and large-scale write-heavy workloads

### [[Graph Databases]]

- [ ] Model entities and relationships as **nodes and edges**
- [ ] Use cases: recommendation, fraud detection, social networks

### [[Search Engines]]

- [ ] Understand why search engines (Elasticsearch, Solr, OpenSearch) are often treated as databases
- [ ] Learn concepts: **inverted index, relevance scoring**

### [[Time-Series Databases]]

- [ ] Understand time-series workloads: metrics, logs, events
- [ ] Learn patterns like **downsampling, retention policies**

### [[Vector Databases]]

- [ ] Grasp embeddings and **similarity search** (kNN)
- [ ] Understand how vector DBs help with **AI/ML** and semantic search

---

## 🔗 Connections

- Reuse fundamentals from [[01 - Fundamentals]]: sharding, replication, CAP
- Compare NoSQL trade-offs with [[02 - RDBMS]]
- Connect to [[07 - Data Modeling]] for polyglot persistence and microservice patterns
