# Practice Projects

End-to-end projects that connect multiple topics across this roadmap. Treat these as **mini capstones** to move from theory to real-world skills.

---

## 1. OLTP E‑Commerce System (PostgreSQL)

**Goal:** Design and build a small but realistic online store backend using a relational database.

### Topics Used

- [01 - Fundamentals](01%20-%20Fundamentals.md) – ACID, Transactions & Isolation, Indexes, Query Optimization
- [02 - RDBMS](02%20-%20RDBMS.md) – [PostgreSQL](02%20-%20RDBMS/PostgreSQL.md) and [Concepts](02%20-%20RDBMS/Concepts.md)
- [07 - Data Modeling](07%20-%20Data%20Modeling.md) – [ER Modeling](07%20-%20Data%20Modeling/ER%20Modeling.md), normalization, basic [Star Schema](07%20-%20Data%20Modeling/Star%20Schema.md) for simple reports

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

- [04 - Big Data](04%20-%20Big%20Data.md) – [Distributed Storage](04%20-%20Big%20Data/Distributed%20Storage.md), [Data Warehouses](04%20-%20Big%20Data/Data%20Warehouses.md), [Query Engines](04%20-%20Big%20Data/Query%20Engines.md)
- [07 - Data Modeling](07%20-%20Data%20Modeling.md) – [Star Schema](07%20-%20Data%20Modeling/Star%20Schema.md), [Snowflake Schema](07%20-%20Data%20Modeling/Snowflake%20Schema.md), [SCD Types](07%20-%20Data%20Modeling/SCD%20Types.md)

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

- [03 - NoSQL](03%20-%20NoSQL.md) – [Time-Series Databases](03%20-%20NoSQL/Time-Series%20Databases.md), possibly [Wide-Column Stores](03%20-%20NoSQL/Wide-Column%20Stores.md)
- [04 - Big Data](04%20-%20Big%20Data.md) – [Streaming Systems](04%20-%20Big%20Data/Streaming%20Systems.md)

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

- [03 - NoSQL](03%20-%20NoSQL.md) – [Document Stores](03%20-%20NoSQL/Document%20Stores.md), [Key-Value Stores](03%20-%20NoSQL/Key-Value%20Stores.md)
- [07 - Data Modeling](07%20-%20Data%20Modeling.md) – [Polyglot Persistence](07%20-%20Data%20Modeling/Polyglot%20Persistence.md), [Microservice DB Patterns](07%20-%20Data%20Modeling/Microservice%20DB%20Patterns.md), [CQRS](07%20-%20Data%20Modeling/CQRS.md), [Event Sourcing](07%20-%20Data%20Modeling/Event%20Sourcing.md)
- [05 - Cloud Databases](05%20-%20Cloud%20Databases.md) – one managed DB of your choice

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

- [08 - Modern Databases](08%20-%20Modern%20Databases.md) – [Google Spanner](08%20-%20Modern%20Databases/Google%20Spanner.md), [CockroachDB](08%20-%20Modern%20Databases/CockroachDB.md), [YugabyteDB](08%20-%20Modern%20Databases/YugabyteDB.md), [TiDB](08%20-%20Modern%20Databases/TiDB.md), [PlanetScale](08%20-%20Modern%20Databases/PlanetScale.md), [SingleStore](08%20-%20Modern%20Databases/SingleStore.md)
- [06 - Internals](06%20-%20Internals.md) – [Raft Consensus](06%20-%20Internals/Raft%20Consensus.md), [B-Tree vs LSM](06%20-%20Internals/B-Tree%20vs%20LSM.md), [2PC & 3PC](06%20-%20Internals/2PC%20&%203PC.md)
- [01 - Fundamentals](01%20-%20Fundamentals.md) – [CAP Theorem](01%20-%20Fundamentals/CAP%20Theorem.md), [Sharding](01%20-%20Fundamentals/Sharding.md), [Replication](01%20-%20Fundamentals/Replication.md)

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
