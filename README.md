### Hi there, I'm Anurag

<a href="https://x.com/AnuragThePathak" target="_blank" rel="noopener noreferrer">
  <img align="left" width="40px" src="./images/x.svg" />
</a>
<a href="https://www.linkedin.com/in/anuragthepathak/" target="_blank" rel="noopener noreferrer">
  <img align="left" width="40px" src="./images/linkedin.svg" />
</a>
<a href="mailto:contact@anuragthepathak.com" target="_blank" rel="noopener noreferrer">
  <img align="left" width="43px" src="./images/gmail.svg" />
</a>

<br><br>

### About Me 🚀

👨‍💻 **Backend Engineer & Systems Thinker** <br>
I build backend systems with a focus on predictability, explicit boundaries, and code that reads like it explains itself—simple by choice, not by limitation. 

⚡ I actively build in the upstream cloud-native ecosystem, contributing core infrastructure features to Kubernetes-SIGs and CNCF projects. <br>
🙋‍♂️ I enjoy sharing what I learn along the way and helping others reason about distributed systems more clearly. 

I'm a "forever Go" developer drawn to the **cloud-native ecosystem**.  
I evaluate system design through the lens of:
- **Strict Bounded Contexts:** enforcing contracts so domains never leak.
- **Predictability over Magic:** strong typing, explicit dependency injection, and **graceful degradation**.
- **Enterprise Observability:** treating distributed tracing and structured logs as core application features, not afterthoughts.
- **Preventive Design:** designing things *right* so they don't become painful at 3:00 AM under heavy load.

---

### 🏆 Featured Architecture 

**[Subscription Management Service](https://github.com/AnuragThePathak/subscription-management)** A production-grade Go backend built to demonstrate strict domain boundaries and resilient infrastructure.  
- **Observability & Tracing:** End-to-end instrumentation (Metrics, Structured Logs, and Traces) across HTTP handlers, Redis, MongoDB, and Asynq. Features automatic trace-correlated slog logging and native W3C trace context propagation bridging the Queue-to-Worker event boundary.
- **Adversarial Testing:** Defense-in-depth test suite utilizing Testcontainers, pre-poisoned database decoys, and mutation-preventing domain tests to mathematically verify queries.
- **Resilience:** Implemented fail-open Redis rate limiting to prioritize core API availability during cache degradation.

---

### ✍️ Technical Writing

I occasionally write about infrastructure and my open-source learnings.
- [How I Passed the CKA Exam on My First Attempt](https://anuragpathak.hashnode.dev/how-i-passed-the-cka-exam-in-the-first-attempt)
- [My LFX Mentorship Experience with OpenELB (CNCF)](https://dev.to/anuragpathak/my-lfx-mentorship-experience-with-openelb-4mhn)

---

### 🛠️ Primary Focus

**Backend & Systems**: Clean architecture, domain-driven design, explicit state machines.
<br>
![Go](https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white)

**Observability & Data**: 
<br>
![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=for-the-badge&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/redis-%23DD0031.svg?style=for-the-badge&logo=redis&logoColor=white)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-000000.svg?style=for-the-badge&logo=opentelemetry&logoColor=white)
![Grafana](https://img.shields.io/badge/grafana-%23F46800.svg?style=for-the-badge&logo=grafana&logoColor=white)

**Cloud-Native & Tooling**: 
<br>
![Kubernetes](https://img.shields.io/badge/kubernetes-%23326ce5.svg?style=for-the-badge&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)

---

### 📌 Current Focus

- **Kubernetes Operator Patterns**: Exploring advanced controller-runtime mechanics, indexing, and fail-closed state reconciliation for highly distributed cloud infrastructure.
- **Graceful Shutdown Topologies:** Architecting deterministic, reverse-order shutdown sequences (via Dependency Injection graphs like `uber-go/fx`) to resolve connection-draining race conditions during SIGTERM.
- **Task Chaining & DLQs:** Decoupling domain mutations from external side-effects (e.g., separating billing logic from SMTP notifications) using Asynq task chaining and Dead Letter Queues.
- **Caching Strategies:** Expanding Redis implementations strictly for database query offloading and read-heavy endpoint optimization.
- **E2E Verification:** Expanding hermetic testing strategies into full End-to-End (E2E) request lifecycle verification.
