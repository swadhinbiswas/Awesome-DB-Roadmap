# 06 – Database Internals

This is where you learn what’s happening **under the hood**.

---

## 📌 Overview

- [ ] Understand how storage, indexing, logging, and coordination work internally
- [ ] Build mental models that make performance tuning intuitive

---

## 🧠 Core Internal Topics

### [[B-Tree vs LSM]]

- [ ] Compare write/read patterns of B-Tree and LSM
- [ ] Understand compaction, write amplification, and read amplification

### [[Buffer Pools]]

- [ ] Learn how in-memory pages cache disk blocks
- [ ] Understand eviction policies (LRU, clock, etc.)

### [[WAL Internals]]

- [ ] See how logs ensure durability and crash recovery

### [[Query Planner]]

- [ ] Understand how logical queries become physical execution plans
- [ ] Learn about join strategies, scan types, and cost models

### [[MVCC Internals]]

- [ ] Dive deeper into snapshots, versions, and garbage collection

### [[Raft Consensus]]

- [ ] Understand key ideas of log replication and leader election

### [[Paxos]]

- [ ] Learn the theory behind consensus in distributed systems

### [[2PC & 3PC]]

- [ ] Understand distributed transactions and commit protocols

### [[Hashing & Bloom Filters]]

- [ ] Learn how probabilistic data structures speed up lookups and joins

---

## 🔗 Connections

- Deepens concepts from [[01 - Fundamentals]] and [[02 - RDBMS]]
- Provides the foundation for [[08 - Modern Databases]] designs
