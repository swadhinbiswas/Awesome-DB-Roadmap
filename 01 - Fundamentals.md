# 01 – Fundamentals

Foundational ideas that power **all** database systems, regardless of technology.

---

## 📌 Overview

- [ ] Understand **why databases exist** and what problems they solve
- [ ] Grasp the trade-offs between **consistency, availability, and performance**
- [ ] Learn how databases maintain **correctness** even with failures and concurrency

---

## 🧱 Core Topics

### [[ACID]]

- [ ] Define **Atomicity, Consistency, Isolation, Durability**
- [ ] Recognize ACID in real-world scenarios (bank transfers, orders)
- [ ] Understand how ACID relates to **transactions** and **constraints**

### [[CAP Theorem]]

- [ ] Learn what **Consistency, Availability, Partition Tolerance** mean in practice
- [ ] Understand why under partition, you must trade **C vs A**
- [ ] Map real systems (e.g., Cassandra, MongoDB, Spanner) onto CAP choices

### [[Transactions & Isolation]]

- [ ] Understand what a **transaction** is and why we need it
- [ ] Learn isolation levels: **Read Uncommitted, Read Committed, Repeatable Read, Serializable**
- [ ] Recognize anomalies: **dirty reads, non-repeatable reads, phantom reads**

### [[Concurrency Control]]

- [ ] Understand **locks**, **latches**, and **optimistic vs pessimistic** control
- [ ] Learn about **deadlocks** and how systems detect/avoid them
- [ ] Connect concurrency control to **isolation levels**

### [[Indexes]]

- [ ] Explain what an **index** is and why it speeds up queries
- [ ] Compare **B-Tree** vs **hash** indexes at a high level
- [ ] Understand trade-offs: **read vs write performance**, extra storage, maintenance

### [[Query Optimization]]

- [ ] Understand what a **query planner/optimizer** does
- [ ] Read and interpret a simple **EXPLAIN plan**
- [ ] Recognize common anti-patterns (SELECT \*) and how indexes help

### [[Sharding]]

- [ ] Learn what **horizontal partitioning / sharding** means
- [ ] Compare **range**, **hash**, and **directory** sharding
- [ ] Understand challenges: **resharding, hotspots, cross-shard joins**

### [[Replication]]

- [ ] Understand **leader-follower**, **multi-leader**, and **leaderless** replication
- [ ] Learn about **synchronous vs asynchronous** replication
- [ ] Connect replication to **high availability** and **read scaling**

### [[Caching]]

- [ ] Understand why caches exist: **latency** and **load reduction**
- [ ] Compare **in-process**, **near-cache**, and **distributed** caches
- [ ] Learn about **cache invalidation** strategies and consistency issues

### [[Storage Engines]]

- [ ] Understand the difference between a **database** and its **storage engine**
- [ ] Compare high-level characteristics of **B-Tree** and **LSM-tree**-based engines
- [ ] Connect engines to workloads: **OLTP vs OLAP** patterns

### [[WAL & MVCC]]

- [ ] Learn what a **Write-Ahead Log (WAL)** is and why it’s critical
- [ ] Understand **MVCC (Multi-Version Concurrency Control)** at a conceptual level
- [ ] Relate MVCC to **snapshots**, **readers vs writers**, and isolation

---

## 🔗 Next Steps

- After this module, you’re ready to go deeper into:
  - [[02 - RDBMS]] for relational systems
  - [[03 - NoSQL]] for non-relational paradigms
  - [[06 - Internals]] when you want to understand how engines are built
