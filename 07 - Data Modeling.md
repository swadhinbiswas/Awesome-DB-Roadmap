# 07 – Data Modeling & Architecture

Good data modeling separates **junior** from **senior** engineers. This module is about designing data to serve the business.

---

## 📌 Overview

- [ ] Learn to translate real-world requirements into robust schemas
- [ ] Understand trade-offs between **normalized** and **denormalized** models
- [ ] Design for analytics, OLTP, and microservices

---

## 🧱 Modeling Topics

### [[ER Modeling]]

- [ ] Identify entities, relationships, and attributes
- [ ] Draw ER diagrams from real-world domains

### [[Star Schema]]

- [ ] Understand facts and dimensions
- [ ] Learn when star schemas fit analytics workloads

### [[Snowflake Schema]]

- [ ] See how further normalization changes joins and storage

### [[SCD Types]]

- [ ] Learn Slowly Changing Dimensions (Type 1, 2, 3,...)
- [ ] Model historical changes in data warehouses

### [[Event Sourcing]]

- [ ] Model state as a sequence of events

### [[CQRS]]

- [ ] Separate read and write models for scalability and clarity

### [[Polyglot Persistence]]

- [ ] Use multiple databases for different parts of the system

### [[Microservice DB Patterns]]

- [ ] Learn patterns: database-per-service, shared DB, saga, outbox

---

## 🔗 Connections

- Builds on [[02 - RDBMS]] and [[03 - NoSQL]]
- Directly used in [[04 - Big Data]] warehouses and [[05 - Cloud Databases]]
