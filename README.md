# Hi, I'm Davit Ioramashvili

Backend engineer in Tbilisi building **Java / Spring Boot** services, with a focus on reliability: message processing that doesn't lose or double-count data, clean APIs, and well-tested code.

- 🏦 **Basisbank:** I investigate production incidents across core banking systems (cards, transfers, payments) and optimize SQL Server queries.
- ⚙️ **Akvelon:** I triage and investigate issues for a large CI/CD platform in an international team, and work with AI-agent triage workflows.
- 🤖 **AI-assisted development:** I use Claude Code as a directed tool. I break work into small tasks, choose between proposed designs, and require tests and a green build before every commit.

---

## Tech Stack

**Backend:** Java 21 · Spring Boot · Spring MVC · Spring Data JPA / Hibernate · Spring Security · Spring AMQP · REST APIs
**Data & messaging:** PostgreSQL · SQL Server (T-SQL) · MongoDB · Redis · RabbitMQ · Caffeine
**Testing:** JUnit 5 · Mockito · MockMvc · Spring Boot test slices · JaCoCo
**Tools:** Git · Docker · GitHub Actions · Maven · Linux · Claude Code · GitHub Copilot

---

## Featured Projects

### ⚡ [Event-Driven Transaction Statistics Service](https://github.com/dioramashvili/ops-statistics-service)
Spring Boot 4 / Java 21 worker that consumes transaction events from RabbitMQ and aggregates statistics in SQL Server.
- Manual acks, bounded retries with exponential backoff, and a persisted dead-letter queue
- Idempotent processing with a message-ID ledger inside a single transaction
- Concurrency-safe T-SQL upserts and a Caffeine cache with TTL and size limits
- Built with Claude Code, guided by a [CLAUDE.md](https://github.com/dioramashvili/ops-statistics-service/blob/main/CLAUDE.md) that documents the architecture and conventions

### 🛒 [Shop API](https://github.com/dioramashvili/shop-api)
Spring Boot 3 REST API for a product catalog.
- Spring Data JPA / Hibernate with `@EntityGraph` queries to avoid N+1 selects
- Role-based Spring Security with BCrypt, plus Actuator health checks and Micrometer metrics
- 56 unit and integration tests with JaCoCo coverage, and dev/test/prod profiles (H2 / PostgreSQL)

### 🎯 [CareerSim (Ascend.AI)](https://github.com/dioramashvili/Ascend.AI)
Team capstone for *Building AI-Powered Applications* at Kutaisi International University: an LLM-based career simulator that generates workplace scenarios and scores user decisions.
- Multi-provider LLM layer (Gemini with DeepSeek fallback), structured JSON outputs validated with Pydantic
- My part: repository owner and maintainer. I set up the project structure, wrote specs, reviewed and merged the team's pull requests, and handled deployment

### ♟️ [Chess PGN Validator](https://github.com/dioramashvili/chess-pgn-validator)
Java parser and rules engine that validates chess games in PGN format, including castling, en passant, promotion and check/checkmate. Uses a modular OOP design, multithreaded processing of large files, and 31 unit tests.

---

## Currently Learning

Kafka · microservices with Docker · OAuth2 / JWT

---

## Contact

📧 dioramashvili@gmail.com · 🔗 [LinkedIn](https://linkedin.com/in/dioramashvili)
