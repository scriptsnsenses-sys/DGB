# DGB

### A lightweight, modern, open-source relational database engine.

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![Status](https://img.shields.io/badge/Status-Early%20Development-orange.svg)](#roadmap)
[![Open Source](https://img.shields.io/badge/Open%20Source-Yes-brightgreen.svg)](#)

**DGB** is an independent, lightweight relational database engine designed to deliver efficient data storage, optimized query execution, and minimal resource consumption.

Inspired by the accessibility of MySQL and the simplicity of modern database systems, [ProjectName] aims to provide a streamlined database experience without unnecessary complexity.

**Less overhead. Efficient execution. More control.**

---

## 🚀 Vision

Not every application needs the complexity and resource requirements of a traditional database system.

DGB aims to build a modern alternative focused on:

- Lightweight resource consumption.
- Efficient SQL query execution.
- A modular and maintainable architecture.
- Familiar SQL syntax.
- Optional MySQL protocol compatibility.
- Straightforward installation and deployment.
- Open-source development and transparency.

This is not intended to be another MySQL fork. The goal is to develop an independent database engine with its own architecture and implementation.

## ✨ Core Features

Planned capabilities:

| Feature | Description | Status |
|---|---|---|
| SQL Parser | Parse and validate SQL statements | Planned |
| Query Engine | Execute SQL queries efficiently | Planned |
| Storage Engine | Persistent data storage | Planned |
| Indexing | Efficient data retrieval | Planned |
| Transactions | Reliable transactional operations | Planned |
| MySQL Protocol | Compatibility with MySQL clients | Planned |
| Multi-Connection | Concurrent connection support | Planned |
| CLI | Interactive database interface | Planned |
| Configuration | Simple database configuration | Planned |

*Features are subject to development and testing.*

## 🏗️ Architecture

The engine is designed around modular components.

```text
              CLIENT APPLICATIONS
                      |
                      v
               CONNECTION LAYER
                      |
                      v
               PROTOCOL HANDLER
                      |
                      v
                  SQL PARSER
                      |
                      v
                 QUERY ENGINE
                      |
             +--------+--------+
             |                 |
             v                 v
        INDEX ENGINE      TRANSACTION
             |             MANAGER
             +--------+--------+
                      |
                      v
                STORAGE ENGINE
                      |
                      v
                 DISK STORAGE
```

Each component is intended to remain independent, allowing individual subsystems to be optimized and extended.

## 🎯 Design Principles

### 1. Lightweight by Design

Minimize unnecessary dependencies, background processes, and memory overhead.

### 2. Performance Focused

Prioritize efficient query planning, indexing, storage access, and execution.

### 3. Compatibility Where It Matters

Support familiar SQL syntax and explore MySQL protocol compatibility without sacrificing architectural independence.

### 4. Simplicity

Provide sensible defaults, understandable configuration, and straightforward deployment.

### 5. Open Source

Keep development transparent and encourage community contributions.

## 📋 Planned SQL Support

Initial SQL implementation targets:

```sql
CREATE DATABASE example;

USE example;

CREATE TABLE users (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    age INT
);

INSERT INTO users VALUES
(1, 'Daivik', 13);

SELECT * FROM users;

UPDATE users
SET age = 14
WHERE id = 1;

DELETE FROM users
WHERE id = 1;
```

Additional planned capabilities:

- WHERE conditions
- ORDER BY
- GROUP BY
- JOIN operations
- Aggregate functions
- Secondary indexes
- Transaction support

## ⚡ Performance Philosophy

Performance is a design objective, not an unverified marketing claim.

The project intends to measure:

- Memory consumption.
- CPU utilization.
- Database startup time.
- Query latency.
- Concurrent connection performance.
- Storage efficiency.

Benchmarks will be published with reproducible configurations and comparisons.

## 🛠️ Installation

Installation instructions will be published with the first development release.

**Currently, the project is under active development.**

## 🗺️ Roadmap

- [ ] Establish core architecture.
- [ ] Implement SQL tokenizer.
- [ ] Implement SQL parser.
- [ ] Build basic query execution.
- [ ] Implement persistent storage.
- [ ] Add indexing.
- [ ] Introduce transaction support.
- [ ] Develop interactive CLI.
- [ ] Add connection management.
- [ ] Explore MySQL protocol compatibility.
- [ ] Publish initial development release.
- [ ] Work towards a stable production release.

## 🤝 Contributing

Contributions, suggestions, bug reports, and architectural discussions are welcome.

Before submitting substantial changes, open an issue to discuss the proposed implementation.

Please ensure contributions follow the project's coding standards and licensing requirements.

## 🔒 Reliability and Security

Database reliability and data integrity are important development priorities.

Development will focus on:

- Input validation.
- Safe query execution.
- Transaction integrity.
- Concurrent access safety.
- Crash recovery.
- Reliable persistent storage.

Experimental builds should not be used for critical production data.

## 📄 License

Copyright © 2026 DGB Contributors.

This project is licensed under the **Apache License 2.0**.

You are free to use, modify, distribute, and contribute to this project under the terms and conditions of the license.

See the [LICENSE](LICENSE) file for the complete license text.

[![Apache License 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)

---

<div align="center">

**DGB**

*Lightweight by design. Independent by architecture.*

</div>
