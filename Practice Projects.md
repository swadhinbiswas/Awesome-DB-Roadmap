# Practice Projects

End-to-end projects that connect multiple topics across this roadmap. Treat these as **mini capstones** to move from theory to real-world skills.

---

## 1. OLTP E‑Commerce System (PostgreSQL)

**Goal:** Design and build a small but realistic online store backend using a relational database.

### Topics Used

- [[01 - Fundamentals]] – ACID, Transactions & Isolation, Indexes, Query Optimization
- [[02 - RDBMS]] – [[PostgreSQL]] and [[Concepts]]
- [[07 - Data Modeling]] – [[ER Modeling]], normalization, basic [[Star Schema]] for simple reports

### Checklist

- [ ] Model products, users, orders, order_items with an ER diagram
- [ ] Design a normalized relational schema and create it in PostgreSQL
- [ ] Add appropriate indexes (PKs, FKs, and query-specific indexes)
- [ ] Implement typical workflows:
  - [ ] User registration and login
  - [ ] Create order with multiple items (single transaction)
  - [ ] Payment success/failure and rollback behavior
- [ ] Use `EXPLAIN ANALYZE` to tune at least 3 queries
- [ ] Write a short note reflecting where ACID and isolation levels appear

---

## 2. Analytics Warehouse for the Store

**Goal:** Extend the e‑commerce system with a basic analytics pipeline and warehouse.

### Topics Used

- [[04 - Big Data]] – [[Distributed Storage]], [[Data Warehouses]], [[Query Engines]]
- [[07 - Data Modeling]] – [[Star Schema]], [[Snowflake Schema]], [[SCD Types]]

### Checklist

- [ ] Define analytical questions (e.g., revenue per day, top products, retention)
- [ ] Design a star schema: one fact table (orders or order_lines), several dimensions
- [ ] Build the schema in a warehouse (Snowflake/BigQuery/Redshift or even PostgreSQL)
- [ ] Load data from OLTP DB into the warehouse (can be CSV export + COPY)
- [ ] Implement at least 5 analytics queries and save them as examples
- [ ] Experiment with one SCD Type 2 dimension (e.g., customer profile changes)

---

## 3. Real‑Time Metrics & Time‑Series

**Goal:** Collect and analyze time-based metrics like page views or application logs.

### Topics Used

- [[03 - NoSQL]] – [[Time-Series Databases]], possibly [[Wide-Column Stores]]
- [[04 - Big Data]] – [[Streaming Systems]]

### Checklist

- [ ] Instrument a simple app or script to emit events (e.g., page_view)
- [ ] Use a stream (e.g., Kafka) or simple queue to collect events
- [ ] Store data in a time-series DB (InfluxDB/TimescaleDB/Prometheus-like)
- [ ] Define retention and downsampling strategy
- [ ] Build at least 3 time-based dashboards/queries (e.g., hourly counts)

---

## 4. Polyglot Microservice System

**Goal:** Design a small microservice architecture using more than one type of database.

### Topics Used

- [[03 - NoSQL]] – [[Document Stores]], [[Key-Value Stores]]
- [[07 - Data Modeling]] – [[Polyglot Persistence]], [[Microservice DB Patterns]], [[CQRS]], [[Event Sourcing]]
- [[05 - Cloud Databases]] – one managed DB of your choice

### Checklist

- [ ] Choose a domain (e.g., task management, social posts)
- [ ] Split into 2–3 services (e.g., users, posts, analytics)
- [ ] Give each service its own data store (RDBMS, document store, KV cache)
- [ ] Model one workflow with CQRS and/or event sourcing
- [ ] Implement a basic saga or outbox pattern for cross-service consistency

---

## 5. Distributed SQL Exploration

**Goal:** Explore a modern distributed SQL database and connect theory to practice.

### Topics Used

- [[08 - Modern Databases]] – [[Google Spanner]], [[CockroachDB]], [[YugabyteDB]], [[TiDB]], [[PlanetScale]], [[SingleStore]]
- [[06 - Internals]] – [[Raft Consensus]], [[B-Tree vs LSM]], [[2PC & 3PC]]
- [[01 - Fundamentals]] – [[CAP Theorem]], [[Sharding]], [[Replication]]

### Checklist

- [ ] Pick one distributed SQL system (local or cloud trial)
- [ ] Create a small schema and load sample data
- [ ] Observe how it handles replication and failover (docs or simple tests)
- [ ] Run queries that span multiple nodes/regions (if supported)
- [ ] Write a short comparison against a single-node RDBMS (PostgreSQL/MySQL)

---

## How to Use These Projects

- Don’t try to do all projects at once; pick **one** that aligns with your current focus.
- As you work, keep relevant topic notes (e.g., `ACID`, `Indexes`, `Event Sourcing`) open side by side.
- Use checkboxes here _and_ in concept notes to track both theory and practice.
- After finishing a project, write a short **retrospective note** on what you learned and what hurt—that’s where the senior-level insight comes from.
