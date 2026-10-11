# 180-Day Roadmap

## How to use this roadmap

Day 0 is a pre-roadmap reset. The numbered 180-day journey starts at Day 1. Use the phase outcomes below as milestones, not as a reason to rush past gaps. Adjust individual days when a topic needs more practice, but record the change in `PROGRESS.md`.

## Phase overview

| Phase | Days | Focus | Target evidence |
|---|---:|---|---|
| Day 0 | Preparation | JavaScript, TypeScript, Git/GitHub reset | Solved exercises, Git lab, first pull request |
| Month 1 | 1–28 | Node.js, TypeScript, backend engineering | Typed API/service project with tests |
| Month 2 | 29–56 | PostgreSQL, Redis, Kafka, data consistency | Order-processing service and integration tests |
| Month 3 | 57–84 | Docker, cloud, CI/CD, delivery, system design | Deployed service and automated pipeline |
| Month 4 | 85–112 | Kubernetes, Terraform, platform engineering | Reproducible infrastructure and deployment |
| Month 5 | 113–154 | Distributed systems, system design, applied AI/LLM | RAG/LLM project with evaluation and guardrails |
| Month 6 | 155–180 | Capstone, reliability, DSA, interviews | Multi-tenant internal developer platform |

## Day 0 — JS + TS + Git/GitHub reset

**Purpose:** regain coding fluency and establish the repository workflow before Month 1.

### Suggested 5–6 hour schedule

| Time | Focus | Deliverable |
|---|---|---|
| 20 min | Check Node.js, npm, Git, VS Code, GitHub authentication | Environment checklist |
| 70 min | JS fundamentals, functions, closures, arrays, objects | JavaScript exercises |
| 45 min | Promises, `async/await`, event-loop prediction, retry | Async exercises |
| 60 min | TS types, unions, narrowing, generics, `keyof`, `unknown`, `never` | Typed exercises |
| 75 min | Git status/add/diff/commit/branch/merge/remote/push | Basic Git lab |
| 45 min | Restore/reset/revert/stash/reflog in a disposable repo | Recovery notes |
| 25 min | Review, update progress, push changes | Day 0 checkpoint |

Split this over two sessions if necessary. Avoid turning the reset into a long detour.

### JavaScript checklist

- [ ] Explain `var`, `let`, `const`, hoisting, and the temporal dead zone.
- [ ] Explain `==` vs `===`, truthiness, coercion, `??`, and optional chaining.
- [ ] Implement a closure-based counter, `once`, and `memoize`.
- [ ] Transform/group data with `map`, `filter`, and `reduce`.
- [ ] Explain shallow copies and immutable updates.
- [ ] Predict promise, microtask, and timer ordering.
- [ ] Compare sequential `await` with `Promise.all`.
- [ ] Implement bounded retry with exponential backoff.

### TypeScript checklist

- [ ] Model `ApiResponse<T>` and `Result<T, E>`.
- [ ] Implement `getProperty<T, K extends keyof T>(obj, key)`.
- [ ] Implement a generic in-memory `Repository<T>`.
- [ ] Use discriminated unions and exhaustive checking.
- [ ] Explain `any` vs `unknown`, `never`, and type narrowing.
- [ ] Explain why compile-time types do not replace runtime validation.

### Git/GitHub checklist

- [ ] Configure `user.name` and `user.email`.
- [ ] Explain working directory, staging area, local repository, and remote.
- [ ] Practise `status`, `add`, `diff`, `diff --staged`, `commit`, and `log`.
- [ ] Create a feature branch, commit work, merge it, and inspect the graph.
- [ ] Connect a local repository to GitHub and push a branch.
- [ ] Open and review a pull request.
- [ ] Explain `restore` vs `reset` vs `revert`.
- [ ] Practise `stash` and `reflog` in a disposable repository.
- [ ] Explain why `reset --hard` and force-push require care.

## Month 1 — Node.js, TypeScript, backend engineering (Days 1–28)

**Outcome:** build and explain a typed backend service with clean boundaries, validation, authentication/security basics, logging, and automated tests.

Suggested project progression:
- Node.js runtime, event loop, modules, npm, and process behavior.
- Async patterns, concurrency limits, streams, and error handling.
- Advanced TypeScript, API contracts, validation, and reusable abstractions.
- HTTP/REST, layered architecture, authentication, authorization, and security basics.
- Unit/integration tests, structured logs, configuration, and documentation.
- Integrate the work into a typed REST API/authentication service.

## Month 2 — Data and messaging (Days 29–56)

**Outcome:** build an order-processing system using PostgreSQL, Redis, and Kafka or an equivalent event broker.

Focus areas:
- SQL modelling, indexes, transactions, query plans, migrations.
- Caching, TTLs, invalidation, and cache failure.
- Events, consumer groups, retries, dead-letter handling, idempotency.
- Transaction boundaries, outbox pattern, and consistency trade-offs.
- Integration tests and failure simulations.

## Month 3 — Containers, cloud, CI/CD (Days 57–84)

**Outcome:** package and deploy a service with automated tests, security checks, and a repeatable delivery pipeline.

Focus areas:
- Docker images, multi-stage builds, non-root execution, image hygiene.
- Cloud networking, identity/IAM, compute, storage, and managed data services.
- CI pipelines, artifact promotion, secrets, rollback, and deployment strategies.
- Logs, metrics, traces, health checks, and operational runbooks.
- Document architecture and cost/security trade-offs.

## Month 4 — Kubernetes and platform engineering (Days 85–112)

**Outcome:** deploy workloads on Kubernetes and provision infrastructure reproducibly.

Focus areas:
- Pods, Deployments, Services, Ingress/Gateway, ConfigMaps, Secrets.
- Probes, requests/limits, autoscaling, rollout and rollback.
- RBAC, network policy, workload identity, resource isolation.
- Terraform modules, state, plans, drift, and safe changes.
- Helm/Kustomize and GitOps workflow.
- Troubleshooting drills and operational documentation.

## Month 5 — Distributed systems, system design, applied AI/LLM (Days 113–154)

**Outcome:** demonstrate system-design reasoning and build an AI-enabled application with measurable quality and safe failure behavior.

Focus areas:
- Availability, latency, throughput, partitioning, replication, consistency.
- Timeouts, retries, circuit breakers, backpressure, idempotency, sagas.
- System-design exercises with capacity estimates and trade-offs.
- LLM APIs, embeddings, retrieval-augmented generation (RAG), evaluation.
- Tool calling, permissions, prompt-injection awareness, observability, cost/latency controls.
- Build an AI assistant that uses explicit tools and auditable outputs.

## Month 6 — Capstone and interviews (Days 155–180)

**Outcome:** finish a production-minded multi-tenant internal developer platform and prepare to explain its design and operation.

Capstone direction:
- A portal and API for teams to request/manage application environments.
- Node.js/TypeScript API, PostgreSQL, Redis, event-driven workflows.
- Infrastructure as code, Kubernetes, GitOps, and CI/CD.
- Multi-tenancy, RBAC, idempotency, workflow recovery, and audit trails.
- Observability, SLOs, runbooks, failure drills, and security boundaries.
- An AI SRE copilot with bounded, permissioned tools and evaluation.
- Architecture diagrams, ADRs, test evidence, demo, and interview walkthrough.

## Weekly review

At the end of each week:
1. Review the code and tests, not just the notes.
2. Revisit weak topics and unresolved bugs.
3. Explain one design decision and one trade-off aloud.
4. Update `PROGRESS.md` with evidence and the next week's priority.
5. Refactor only when it improves clarity, correctness, or testability.

## Change log

- Initial roadmap created for the Day 0 repository setup.
- Record meaningful changes to the learning sequence here.
