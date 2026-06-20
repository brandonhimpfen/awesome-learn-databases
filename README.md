# Awesome Learn: Databases [![Awesome Learn](https://srv-cdn.himpfen.io/badges/awesome-learn/awesomelearn-flat.svg)](https://github.com/brandonhimpfen/awesome-learn)

[![Support Open Work](https://img.shields.io/badge/Support-Open%20Work-0A0A0A?style=flat&logo=github)](https://github.com/brandonhimpfen/support) 

A curated and structured learning path for Databases.

This repository is part of the Awesome Learn ecosystem. It is designed to help learners move from fundamentals to practical application through a clear, progressive path.

## Template Principles

This learning path follows a simple philosophy:

- Structured over exhaustive
- Curated over crowded
- Progressive over flat
- Practical over theoretical

The goal is not to collect every database resource, but to guide learners through a meaningful sequence from basic data storage concepts to practical database design, querying, scaling, reliability, and operations.

## How to Use This Template

Use this repository as a guided path for learning databases.

Start with the foundations, then move through relational databases, SQL, modeling, indexing, transactions, NoSQL systems, distributed databases, and real-world operational concerns.

You do not need to complete every resource. Focus on understanding the concepts, practicing with real queries, building small schemas, and learning how database choices affect application behavior.

## Learning Path

### 1. Introduction

Databases are systems for storing, organizing, querying, updating, and protecting data.

They sit at the center of most modern applications. A database can power a personal project, a business application, a public API, an analytics platform, a search engine, a messaging system, or a large distributed service.

Learning databases means learning more than one product. It means understanding how data is modeled, how queries are executed, how indexes improve performance, how transactions protect correctness, how systems scale, and how failures are handled.

A strong database learner should be able to answer questions such as:

- What kind of data is being stored?
- How will the data be queried and updated?
- What relationships exist between entities?
- What consistency guarantees are needed?
- What indexes are useful, and what do they cost?
- When is a relational database enough?
- When might a document, key-value, graph, search, or columnar system make sense?
- How should backups, migrations, monitoring, and recovery be handled?

Databases are not just storage tools. They are design decisions that shape reliability, performance, cost, and maintainability.

### 2. Key Areas to Understand

Databases include several connected areas. These topics appear throughout the learning path.

- Data modeling: representing entities, relationships, constraints, and business rules.
- Relational databases: using tables, rows, columns, keys, joins, constraints, and SQL.
- SQL: querying, filtering, joining, grouping, aggregating, inserting, updating, and deleting data.
- Indexes: improving read performance while understanding write and storage tradeoffs.
- Transactions: preserving correctness through atomicity, consistency, isolation, and durability.
- Concurrency: handling multiple reads and writes safely.
- Query planning: understanding how databases execute queries and choose access paths.
- Normalization and denormalization: balancing data integrity, simplicity, and performance.
- NoSQL databases: understanding document, key-value, wide-column, graph, time-series, and search systems.
- Replication: copying data for availability, read scaling, or disaster recovery.
- Partitioning and sharding: splitting data across machines or logical boundaries.
- Backups and recovery: protecting data against loss, corruption, deletion, or outages.
- Migrations: changing schemas safely as applications evolve.
- Observability: monitoring database health, performance, capacity, and errors.
- Security and privacy: protecting credentials, access, sensitive data, and audit trails.

### 3. Foundations

Begin by learning what databases do and how data is represented.

Core concepts:

- Tables, documents, records, keys, and values
- Entities and relationships
- Primary keys and foreign keys
- CRUD operations
- Schemas and schema-less designs
- Constraints and validation
- Basic SQL syntax
- Reads, writes, latency, and throughput
- Database clients and connections
- Data integrity and durability

Recommended starting exercises:

- Create a small contacts database with people, emails, and phone numbers.
- Model a simple blog with users, posts, categories, and comments.
- Write SQL queries using `SELECT`, `WHERE`, `ORDER BY`, `GROUP BY`, and `JOIN`.
- Compare storing the same data in a relational table and a JSON document.
- Explain why a primary key matters.

Good foundational resources:

- [SQLBolt](https://sqlbolt.com/) - Interactive lessons for learning SQL basics through hands-on examples.
- [PostgreSQL Tutorial](https://www.postgresqltutorial.com/) - Practical tutorials covering PostgreSQL, SQL, tables, joins, indexes, and functions.
- [Use The Index, Luke](https://use-the-index-luke.com/) - A clear guide to SQL indexing and query performance.

### 4. Intermediate Understanding

After the basics, learn how databases behave under real application conditions.

Key topics:

- Joins and relationship modeling
- One-to-one, one-to-many, and many-to-many relationships
- Normal forms and normalization
- Denormalization for read-heavy workloads
- Index types and composite indexes
- Query execution plans
- Transactions and isolation levels
- Locks and deadlocks
- Connection pooling
- Stored procedures and functions
- Views and materialized views
- Schema migrations
- Backups and restores
- Replication basics
- Read replicas
- Caching with databases
- Search indexes and full-text search

Practice prompts:

- Design a database for an online bookstore.
- Design a database for a task management application.
- Add indexes to improve slow queries in a blog database.
- Explain the tradeoff between normalized and denormalized order data.
- Compare PostgreSQL and MongoDB for a content management system.
- Create a migration plan for adding a required field to an existing table.

Useful resources:

- [PostgreSQL Documentation](https://www.postgresql.org/docs/) - Official documentation for PostgreSQL concepts, SQL features, administration, indexing, and performance.
- [MySQL Documentation](https://dev.mysql.com/doc/) - Official documentation for MySQL usage, administration, storage engines, replication, and optimization.
- [MongoDB Manual](https://www.mongodb.com/docs/manual/) - Official documentation for document modeling, querying, indexing, aggregation, and operations.

### 5. Practical Application

Databases become easier to understand when learners connect design decisions to real application needs.

When designing a database, follow a simple process:

1. Clarify the application and users.
2. Identify the main entities.
3. Define relationships between entities.
4. Decide which data must be consistent.
5. Identify common reads and writes.
6. Choose a database type.
7. Design the schema or document model.
8. Define indexes based on query patterns.
9. Plan migrations and version changes.
10. Address backups, recovery, security, and observability.
11. Test performance with realistic data.
12. Document tradeoffs and future risks.

Systems to practice:

- Blog database
- User account database
- Product catalog
- E-commerce order system
- Event registration system
- Inventory system
- Messaging database
- Analytics events database
- Time-series metrics store
- Search-backed document library
- Social graph database
- Audit log database

For each system, write down:

- Entities
- Relationships
- Schema or document structure
- Example queries
- Index choices
- Transaction needs
- Scaling assumptions
- Backup strategy
- Privacy and security concerns
- Migration risks
- Tradeoffs

### 6. Projects

Projects should be small enough to build, but realistic enough to teach database thinking.

#### Project 1: Personal Library Database

Build a database for books, authors, genres, reading status, and notes.

Learn:

- Entity modeling
- Relationships
- Primary and foreign keys
- Basic SQL queries
- Filtering and sorting
- Many-to-many relationships

#### Project 2: Blog Platform Schema

Design a schema for users, posts, comments, tags, and publication status.

Learn:

- Normalization
- Joins
- Constraints
- Slugs and unique fields
- Draft and published states
- Query patterns

#### Project 3: E-commerce Orders Database

Build a database for products, carts, customers, orders, payments, and inventory.

Learn:

- Transactions
- Data consistency
- Order snapshots
- Inventory updates
- Audit trails
- Failure handling

#### Project 4: Analytics Event Store

Create a database for storing page views, user actions, sessions, and basic reports.

Learn:

- Append-only event data
- Time-based queries
- Aggregation
- Partitioning concepts
- Retention policies
- Batch reporting

#### Project 5: Searchable Knowledge Base

Build a small knowledge base with articles, categories, tags, revisions, and search metadata.

Learn:

- Full-text search
- Document metadata
- Versioning
- Indexing
- Access control
- Content lifecycle design

### 7. Resources

Curated list of high-quality resources.

#### Books

- [Designing Data-Intensive Applications](https://dataintensive.net/) - Essential reading for storage engines, replication, partitioning, transactions, distributed systems, and data architecture.
- [Database Internals](https://www.databass.dev/) - A deeper look at how database systems work internally, including storage engines and distributed systems concepts.
- [Readings in Database Systems](http://www.redbook.io/) - A curated collection of important database systems papers with commentary.

#### Courses and Guides

- [CMU Database Group Courses](https://15445.courses.cs.cmu.edu/) - University-level database systems material covering internals, execution, transactions, and storage.
- [SQLBolt](https://sqlbolt.com/) - Beginner-friendly interactive SQL lessons.
- [Mode SQL Tutorial](https://mode.com/sql-tutorial/) - Practical SQL lessons focused on analysis and querying.

#### Documentation

- [PostgreSQL Documentation](https://www.postgresql.org/docs/) - Official PostgreSQL documentation for SQL, administration, indexing, replication, and performance.
- [MySQL Documentation](https://dev.mysql.com/doc/) - Official MySQL documentation for development and administration.
- [SQLite Documentation](https://www.sqlite.org/docs.html) - Official SQLite documentation for a lightweight embedded relational database.
- [MongoDB Manual](https://www.mongodb.com/docs/manual/) - Official MongoDB documentation for document databases.
- [Redis Documentation](https://redis.io/docs/latest/) - Official Redis documentation for key-value storage, caching, streams, and data structures.

#### Concepts and References

- [Use The Index, Luke](https://use-the-index-luke.com/) - Practical guide to indexes and SQL performance.
- [Transaction Isolation Levels](https://www.postgresql.org/docs/current/transaction-iso.html) - PostgreSQL documentation explaining isolation levels and transaction behavior.
- [The Architecture of Open Source Applications: Databases](https://aosabook.org/en/) - Essays and case studies explaining how real systems are built.

#### Tools to Understand

These tools are not required at the beginning, but they commonly appear in database learning and system design discussions.

- PostgreSQL
- MySQL / MariaDB
- SQLite
- MongoDB
- Redis
- Cassandra
- Elasticsearch / OpenSearch
- Neo4j
- InfluxDB
- DuckDB
- ClickHouse
- Supabase
- Prisma
- Flyway
- Liquibase

### 8. Next Steps

After completing this path, continue by building stronger depth in adjacent areas.

Recommended next learning paths:

- SQL
- Data Modeling
- Distributed Systems
- System Design
- Data Engineering
- Search Systems
- Storage Systems
- Site Reliability Engineering
- Cloud Architecture
- Cybersecurity

Ways to keep improving:

- Design schemas for applications you use every day.
- Read database documentation instead of relying only on tutorials.
- Practice explaining why an index helps or hurts a query.
- Load realistic sample data and inspect query plans.
- Compare relational and document models for the same use case.
- Write migration plans before changing schemas.
- Practice backup and restore workflows.
- Read real engineering posts about database failures and scaling decisions.

## Contribution Guidelines

Please read CONTRIBUTING.md before submitting changes.

Contributions should improve clarity, correctness, structure, or learning value. This repository should remain curated and progressive, not exhaustive.

## License

This list is licensed under Creative Commons Zero v1.0 Universal.
