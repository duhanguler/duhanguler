# Duhan Güler

**Software Engineer — Backend, Systems, Database Security & AI Infrastructure**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-duhanguler-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/duhanguler)
[![GitHub](https://img.shields.io/badge/GitHub-duhanguler-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/duhanguler)
[![GitHub Release - spring-dlt-deck](https://img.shields.io/github/v/release/duhanguler/spring-dlt-deck?style=flat-square&label=Java%2025%20%7C%20spring-dlt-deck&color=0284C7&logo=springboot&logoColor=white)](https://github.com/duhanguler/spring-dlt-deck)
[![PyPI - flask-deck](https://img.shields.io/pypi/v/flask-deck?style=flat-square&label=PyPI%20%7C%20flask-deck&color=0D7A52&logo=pypi&logoColor=white)](https://pypi.org/project/flask-deck/)
[![PyPI - flask-lens](https://img.shields.io/pypi/v/flask-lens?style=flat-square&label=PyPI%20%7C%20flask-lens&color=0D7A52&logo=pypi&logoColor=white)](https://pypi.org/project/flask-lens/)
[![PyPI - omrkit](https://img.shields.io/pypi/v/omrkit?style=flat-square&label=PyPI%20%7C%20omrkit&color=0D7A52&logo=pypi&logoColor=white)](https://pypi.org/project/omrkit/)
[![Homebrew Tap](https://img.shields.io/badge/Homebrew-duhanguler%2Ftap-FBB040?style=flat-square&logo=homebrew&logoColor=black)](https://github.com/duhanguler/homebrew-tap)

I design and build high-throughput backend systems, Kafka & database control planes, database wire-protocol proxies, developer observability & operations tooling, cross-platform endpoint agents, and AI/vision pipelines — primarily in **Java 25 (Spring Boot 4.2, Spring Kafka)**, **Python (FastAPI, Flask, Django)**, **Go**, **PostgreSQL**, and **TypeScript**.

Alongside private enterprise and commercial platforms built under NDA, I build public open-source infrastructure and developer tools in **Java**, **Go**, and **Python**.

---

### Open-Source Projects & Developer Tooling

| Project | Domain | Stack | Engineering Highlights |
|---|---|---|---|
| **[spring-dlt-deck](https://github.com/duhanguler/spring-dlt-deck)** | Kafka DLT Triage, Governance & Key-Ordered Replay | Java 25 LTS (`ScopedValue`, `Stream.gather`, JFR, AOT Cache, JEP 519), Spring Boot 4.2, Apache Kafka 4.4 KRaft (KIP-848), PostgreSQL 17, Redis 7 Lua, Spring Security 7, WebMvc.fn, Jackson 3, NullAway, ArchUnit, jqwik, Testcontainers 2, MCP, Helm | Zero-interference drop-in Spring Boot 4.2 starter & standalone control plane for Spring Kafka Dead-Letter Topics (`97.6%` line / `93.8%` branch core coverage, zero global `WebMvcConfigurer`): Two Short TXs + Fencing Tokens + honest `INDETERMINATE` crash semantics (zero DB connections held during Kafka I/O), deterministic multi-pod stripe leasing + Per-Key Head-of-Line Barrier, JEP 290/415 `ObjectInputFilter` poison-pill recovery, Confluent `0x00` `NOT_PATCHABLE` binary guard (`0.178 µs/op`, `~5.6M ops/s`), 3-table hot/cold/deduplicated PostgreSQL schema + SHA-256 batch Merkle checkpoints, checksum-verified PII masking, Honest 3-Tier Dry-Run + bounded RFC 7396 merge patch, four-eyes approval with frozen `planSpecHash` TOCTOU defense, zero-Node Strict Nonce CSP workbench, and ArchUnit-verified fail-closed HITL MCP server. |
| **[pgveil](https://github.com/duhanguler/pgveil)** | Database Security & AI Agent Firewall | Go, PostgreSQL Wire v3, PG17 AST (`pg_query_go`), Virtual RLS, Streamable HTTP MCP, JWT/JWKS, Kafka, Helm/K8s, OpenTelemetry, React | Zero-trust PostgreSQL wire proxy & Streamable HTTP/stdio MCP server ([mcpservers.org](https://mcpservers.org/servers/duhanguler/pgveil)): 8-pack dynamic PII masking (`25k TPS`, `+0.25ms` latency), JWT/JWKS claim-bound AST Virtual Row-Level Security (`{{jwt.*}}`), sideband read-only `EXPLAIN` Cost & Blast-Radius Guard, CTE taint & side-channel oracle defense, unfurl-safe Slack/ChatOps HITL execution holds, zero-config `pgveil demo`, and [Homebrew tap](https://github.com/duhanguler/homebrew-tap). |
| **[flask-deck](https://github.com/duhanguler/flask-deck)** | Enterprise Admin & Operations Workbench | Python 3.10+, Flask, SQLAlchemy 2.0, Strict Nonce CSP, Keyset Pagination, TOTP/OIDC, S3, SSE ([PyPI](https://pypi.org/project/flask-deck/)) | Fail-closed admin & operations platform (`23.6 KB` gzip total, zero Node build / zero CDN, `0 'unsafe-inline'`): pure-Python RFC 6238 TOTP 2FA & SVG QR generator, PKCE `S256` OIDC SSO, HMAC keyset cursor pagination, S3/local media proxy with magic-byte & decompression-bomb guards, native RTL/i18n (`en`/`tr`/`de`/`ar`), soft-delete trash, revision diffs, live SSE background jobs, interactive schema ERD, Kanban & pure SVG analytics (`uvx flask-deck demo`). |
| **[flask-lens](https://github.com/duhanguler/flask-lens)** | Python Observability & Query Guardrails | Python 3.10+, Flask, SQLAlchemy, `cProfile`, SQLite WAL, SSE, Pytest Plugin, PEP 561 Strict ([PyPI](https://pypi.org/project/flask-lens/)) | Two-line Flask DevTools console (`/__lens`) for JSON APIs, HTMX & webhooks (`+0.17ms` SQLAlchemy overhead): automatic SQL N+1 detection with `file:line` callsite attribution, read-only `EXPLAIN` analyzer, zoomable `cProfile` SVG flamegraph, request replay/diff, secret redaction, and Django-style `assert_num_queries` pytest CI guardrails. |
| **[OMRKit (`omr`)](https://github.com/duhanguler/omr)** | Computer Vision & EdTech Platform | Python, OpenCV, NumPy, FastAPI, React, TypeScript, ArUco, QR v3, Docker ([PyPI](https://pypi.org/project/omrkit/) · [Live Studio](https://omrkit-studio.onrender.com/)) | Zero-calibration Optical Mark Recognition engine & 6-language Web Studio: 3-of-4 occluded ArUco 12-point homography recovery, `OMRKIT:v3` QR auto-templating, class-roster mail-merge PDFs, zero-JSON teacher key-sheet scanning, darkness-dominance smudge filtering, Classical Test Theory psychometrics (item difficulty, discrimination & KR-20), Moodle/Canvas LMS exports, and live camera scanner. |

---

### Selected Enterprise & Production Systems *(Private / NDA)*

| System | Domain | Stack | Architecture & Production Highlights |
|---|---|---|---|
| **AI Media Post-Production & GPU Worker Platform** | AI & Media Systems | Python, FastAPI, PyTorch, WhisperX, FFmpeg, React, TypeScript, Redis, PostgreSQL, Docker | Automated speech enhancement & silence cutting, frame-accurate Premiere Pro / DaVinci Resolve XMEML timeline exports, cached 18 TB NAS media gateway, and distributed GPU worker pipeline. |
| **Multi-Tenant AI Video Dubbing & Clipping SaaS** | Multi-Tenant SaaS & AI | Python, Flask, PostgreSQL, Vue 3, RunPod GPU, Demucs, WhisperX, ONNX, FFmpeg, Docker | 11-language synchronized video dubbing & clipping; single-container GPU analysis (<20s per 10-min video), speaker voiceprint matching, real-time SSE job tracking, and 6-tier RBAC. |
| **Enterprise IT Asset Management & Go Endpoint Agent** | Systems & ITAM | Go, PostgreSQL, REST API, SHA-256, S.M.A.R.T. | Cross-platform single-binary endpoint agent (<20 MB RAM) for Windows, Linux & macOS with hardware tamper fingerprinting, SCD Type 2 custody history, and atomic Ed25519/SHA-256 self-updates. |
| **Live Database Backup & Ransomware Protection Engine** | Systems & Security | Windows VSS, SQL, AES-256, S3/R2/B2, SFTP/SMB | Live volume & database snapshotting (MSSQL, MySQL, PostgreSQL), canary decoy-file ransomware halt detection, encrypted 3-2-1 multi-cloud replication, and automated restore verification. |
| **National Association ERP, Billing & Job Marketplace** | Enterprise Web (Flask) | Python, Flask, SQLAlchemy, Alembic, MariaDB, Fernet, WeasyPrint, Nginx | 47-table membership ERP with application-layer PII encryption, HMAC-verified payment callbacks, automated PDF dossier/CV generation, and a two-sided hiring marketplace. |
| **Customs & Bonded Warehouse Management System (WMS)** | Logistics & ERP | Web WMS, Barcode/QR, Android Handhelds, ERP / E-Invoice | 3D rack/bin addressing across customs-bonded and free-storage zones, gate/weighbridge kiosk integration, statutory customs ledgers, and automated ERP e-invoice billing. |

---

### Technical Stack

* **Backend & Web Frameworks:** Java 25 LTS · Spring Boot 4.2 · Spring Framework 7 · Spring Kafka · Spring Security 7 · Hibernate 7 · Python · FastAPI · Flask · Django · Go · SQLAlchemy 2.0 · Alembic · Strawberry GraphQL · REST / Server-Sent Events (SSE)
* **Databases, Storage & Streaming:** PostgreSQL (Wire Protocol v3, PG17 AST, JSONB, Keyset Pagination) · MariaDB / MySQL · SQLite WAL · Apache Kafka 4 (KRaft / KIP-848) / Redpanda · Redis (Lua) · S3 / Cloudflare R2 / Backblaze B2
* **Security & Identity:** OAuth 2.0 / OpenID Connect (PKCE) · JWT / JWKS · WebAuthn / Passkeys · RFC 6238 TOTP · AST SQL Firewalls & Virtual RLS · Strict Nonce CSP · JEP 290 `ObjectInputFilter` · AES-256 / Fernet
* **AI, Media & Computer Vision:** PyTorch (CUDA / MPS) · OpenCV (ArUco, Homography) · WhisperX · Demucs · ONNX · FFmpeg · Model Context Protocol (MCP)
* **Frontend & UI Engineering:** TypeScript · React · Vue 3 · Pinia · Tailwind CSS · Accessible SSR / Zero-Build Vanilla ES6 & SVG Data Visualization
* **Infrastructure, Testing & Observability:** Docker · Kubernetes · Helm · OpenTelemetry · Prometheus · JFR / JMH · Testcontainers 2 · JUnit 6 · ArchUnit · ErrorProne / NullAway · `jqwik` · `cProfile` · Pytest · Mypy / Pyright · Linux · Nginx · GitHub Actions
