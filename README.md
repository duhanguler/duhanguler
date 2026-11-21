# Duhan Güler

**Software Engineer — Backend, Systems, Database Security & AI Infrastructure**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-duhanguler-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/duhanguler)
[![GitHub](https://img.shields.io/badge/GitHub-duhanguler-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/duhanguler)
[![PyPI - omrkit](https://img.shields.io/pypi/v/omrkit?style=flat-square&label=PyPI%20%7C%20omrkit&color=0D7A52&logo=pypi&logoColor=white)](https://pypi.org/project/omrkit/)
[![Homebrew Tap](https://img.shields.io/badge/Homebrew-duhanguler%2Ftap-FBB040?style=flat-square&logo=homebrew&logoColor=black)](https://github.com/duhanguler/homebrew-tap)

I design and build high-throughput backend systems, database wire-protocol proxies, developer observability & operations tooling, cross-platform endpoint agents, and AI/vision pipelines — primarily in **Python (FastAPI, Flask, Django)**, **Go**, **PostgreSQL**, and **TypeScript**.

Alongside private enterprise and commercial platforms built under NDA, I build public open-source infrastructure and developer tools in **Go** and **Python**.

---

### Open-Source Projects & Developer Tooling

| Project | Domain | Stack | Engineering Highlights |
|---|---|---|---|
| **[pgveil](https://github.com/duhanguler/pgveil)** (`v0.4.0`) | Database Security & AI Agent Firewall | Go, PostgreSQL Wire v3, PG17 AST (`pg_query_go`), Virtual RLS, MCP, Kafka, Helm/K8s, OpenTelemetry, React | Zero-trust PostgreSQL wire proxy & native MCP server: 8-pack dynamic PII masking (`25k TPS`, `+0.25ms` latency), AST Virtual Row-Level Security (`Deparse`), CTE taint & side-channel oracle defense, live HITL execution holds, zero-config `pgveil demo`, and [Homebrew tap](https://github.com/duhanguler/homebrew-tap). |
| **[flask-deck](https://github.com/duhanguler/flask-deck)** (`v0.3.0`) | Enterprise Admin & Operations Workbench | Python 3.10+, Flask, SQLAlchemy 2.0, Strict Nonce CSP, Keyset Pagination, TOTP/OIDC, S3, SSE | Fail-closed admin & operations platform (`23.6 KB` gzip total, zero Node build / zero CDN, `0 'unsafe-inline'`): pure-Python RFC 6238 TOTP 2FA & SVG QR generator, PKCE `S256` OIDC SSO, HMAC keyset cursor pagination, S3/local media proxy with magic-byte & decompression-bomb guards, native RTL/i18n (`en`/`tr`/`de`/`ar`), soft-delete trash, revision diffs, live SSE background jobs, interactive schema ERD, Kanban & pure SVG analytics. |
| **[flask-lens](https://github.com/duhanguler/flask-lens)** | Python Observability & Query Guardrails | Python 3.10+, Flask, SQLAlchemy, `cProfile`, SQLite WAL, SSE, Pytest Plugin, PEP 561 Strict | Two-line Flask DevTools console (`/__lens`) for JSON APIs, HTMX & webhooks (`+0.17ms` SQLAlchemy overhead): automatic SQL N+1 detection with `file:line` callsite attribution, read-only `EXPLAIN` analyzer, zoomable `cProfile` SVG flamegraph, request replay/diff, secret redaction, and Django-style `assert_num_queries` pytest CI guardrails. |
| **[OMRKit (`omr`)](https://github.com/duhanguler/omr)** (`v2.3.1`) | Computer Vision & EdTech Platform | Python, OpenCV, NumPy, FastAPI, React, TypeScript, ArUco, QR v3, Docker ([PyPI](https://pypi.org/project/omrkit/) · [Live Studio](https://omrkit-studio.onrender.com/)) | Zero-calibration Optical Mark Recognition engine & 6-language Web Studio: 3-of-4 occluded ArUco 12-point homography recovery, `OMRKIT:v3` QR auto-templating, class-roster mail-merge PDFs, zero-JSON teacher key-sheet scanning, darkness-dominance smudge filtering, Classical Test Theory psychometrics (item difficulty, discrimination & KR-20), Moodle/Canvas LMS exports, and live camera scanner. |

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

* **Backend & Web Frameworks:** Python · FastAPI · Flask · Django · Go · SQLAlchemy 2.0 · Alembic · Strawberry GraphQL · REST / Server-Sent Events (SSE)
* **Databases, Storage & Streaming:** PostgreSQL (Wire Protocol v3, PG17 AST, JSONB, Keyset Pagination) · MariaDB / MySQL · SQLite WAL · Apache Kafka / Redpanda · Redis · S3 / Cloudflare R2 / Backblaze B2
* **Security & Identity:** OAuth 2.0 / OpenID Connect (PKCE) · WebAuthn / Passkeys · RFC 6238 TOTP · AST SQL Firewalls & Virtual RLS · Strict Nonce CSP · AES-256 / Fernet
* **AI, Media & Computer Vision:** PyTorch (CUDA / MPS) · OpenCV (ArUco, Homography) · WhisperX · Demucs · ONNX · FFmpeg · Model Context Protocol (MCP)
* **Frontend & UI Engineering:** TypeScript · React · Vue 3 · Pinia · Tailwind CSS · Accessible SSR / Zero-Build Vanilla ES6 & SVG Data Visualization
* **Infrastructure, Testing & Observability:** Docker · Kubernetes · Helm · OpenTelemetry · Prometheus · `cProfile` · Pytest · Mypy / Pyright · Linux · Nginx · GitHub Actions
