# Cristiano Pacheco

I work on backend systems in Go. My interests include distributed systems, software architecture, and developer tools.

## Selected projects

### [go-shortner](https://github.com/cristiano-pacheco/go-shortner)

A URL shortener with separate processes for redirects and link management.

- Pagination totals use transactional PostgreSQL counters instead of full-table counts.
- Redis lookups fall back to PostgreSQL. Cache entries can remain stale for up to 60 seconds after a change.
- Load tests record throughput, latency, resource limits, and unsuccessful runs.

[Design decisions](https://github.com/cristiano-pacheco/go-shortner/blob/main/docs/architecture.md) · [Benchmarks](https://github.com/cristiano-pacheco/go-shortner/blob/main/docs/performance.md)

### [go-online-auction](https://github.com/cristiano-pacheco/go-online-auction)

A real-time auction system with concurrent bidding and WebSocket updates.

- Row locks, version checks, and domain rules handle competing bids.
- Events are sent after commit through Redis Pub/Sub. Delivery is best effort; the documentation discusses the gap and the outbox alternative.

[Concurrency and events](https://github.com/cristiano-pacheco/go-online-auction#engineering-challenges--solutions) · [Architecture](https://github.com/cristiano-pacheco/go-online-auction#architecture-diagrams)

### [ai-tools](https://github.com/cristiano-pacheco/ai-tools)

Skills, conventions, and tools I use daily with coding agents for planning, implementation, testing, and review. Includes Go architecture guides and reviews against repository standards and specifications.

[Skills](https://github.com/cristiano-pacheco/ai-tools/tree/main/skills/engineering) · [Go architecture guide](https://github.com/cristiano-pacheco/ai-tools/blob/main/docs/go-modular-architecture.md)

---

[LinkedIn](https://www.linkedin.com/in/cristiano-pacheco/) · [Repositories](https://github.com/cristiano-pacheco?tab=repositories) · São Paulo, Brazil
