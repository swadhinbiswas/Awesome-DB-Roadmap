# 01 – Fundamentals

Foundational ideas that power **all** database systems, regardless of technology.

---

## 📌 Overview

- [ ] Understand **why databases exist** and what problems they solve
- [ ] Grasp the trade-offs between **consistency, availability, and performance**
- [ ] Learn how databases maintain **correctness** even with failures and concurrency

---

## 🧱 Core Topics

### [ACID](01%20-%20Fundamentals/ACID.md)

- [ ] Define **Atomicity, Consistency, Isolation, Durability**
- [ ] Recognize ACID in real-world scenarios (bank transfers, orders)
- [ ] Understand how ACID relates to **transactions** and **constraints**

### [CAP Theorem](01%20-%20Fundamentals/CAP%20Theorem.md)

- [ ] Learn what **Consistency, Availability, Partition Tolerance** mean in practice
- [ ] Understand why under partition, you must trade **C vs A**
- [ ] Map real systems (e.g., Cassandra, MongoDB, Spanner) onto CAP choices

### [Transactions & Isolation](01%20-%20Fundamentals/Transactions%20&%20Isolation.md)

- [ ] Understand what a **transaction** is and why we need it
- [ ] Learn isolation levels: **Read Uncommitted, Read Committed, Repeatable Read, Serializable**
- [ ] Recognize anomalies: **dirty reads, non-repeatable reads, phantom reads**

### [Concurrency Control](01%20-%20Fundamentals/Concurrency%20Control.md)

- [ ] Understand **locks**, **latches**, and **optimistic vs pessimistic** control
- [ ] Learn about **deadlocks** and how systems detect/avoid them
- [ ] Connect concurrency control to **isolation levels**

### [Indexes](01%20-%20Fundamentals/Indexes.md)

- [ ] Explain what an **index** is and why it speeds up queries
- [ ] Compare **B-Tree** vs **hash** indexes at a high level
- [ ] Understand trade-offs: **read vs write performance**, extra storage, maintenance

### [Query Optimization](01%20-%20Fundamentals/Query%20Optimization.md)

- [ ] Understand what a **query planner/optimizer** does
- [ ] Read and interpret a simple **EXPLAIN plan**
- [ ] Recognize common anti-patterns (SELECT \*) and how indexes help

### [Sharding](01%20-%20Fundamentals/Sharding.md)

- [ ] Learn what **horizontal partitioning / sharding** means
- [ ] Compare **range**, **hash**, and **directory** sharding
- [ ] Understand challenges: **resharding, hotspots, cross-shard joins**

### [Replication](01%20-%20Fundamentals/Replication.md)

- [ ] Understand **leader-follower**, **multi-leader**, and **leaderless** replication
- [ ] Learn about **synchronous vs asynchronous** replication
- [ ] Connect replication to **high availability** and **read scaling**

### [Caching](01%20-%20Fundamentals/Caching.md)

- [ ] Understand why caches exist: **latency** and **load reduction**
- [ ] Compare **in-process**, **near-cache**, and **distributed** caches
- [ ] Learn about **cache invalidation** strategies and consistency issues

### [Storage Engines](01%20-%20Fundamentals/Storage%20Engines.md)

- [ ] Understand the difference between a **database** and its **storage engine**
- [ ] Compare high-level characteristics of **B-Tree** and **LSM-tree**-based engines
- [ ] Connect engines to workloads: **OLTP vs OLAP** patterns

### [WAL & MVCC](01%20-%20Fundamentals/WAL%20&%20MVCC.md)

- [ ] Learn what a **Write-Ahead Log (WAL)** is and why it’s critical
- [ ] Understand **MVCC (Multi-Version Concurrency Control)** at a conceptual level
- [ ] Relate MVCC to **snapshots**, **readers vs writers**, and isolation

---

## 🔗 Next Steps

- After this module, you’re ready to go deeper into:
  - [02 - RDBMS](02%20-%20RDBMS.md) for relational systems
  - [03 - NoSQL](03%20-%20NoSQL.md) for non-relational paradigms
  - [06 - Internals](06%20-%20Internals.md) when you want to understand how engines are built
