Project 6 — API Gateway and Rate-Limiting Service
Priority: P2

Build a gateway that routes requests to downstream services and applies security and traffic policies.
Stack
- TypeScript and Node.js.
- Redis.
- Docker.
- OpenTelemetry.
- A load-testing tool.
- A small set of mock downstream services.
Modules
- Request routing.
- Authentication and API-key validation.
- Rate limiting.
- Request timeouts.
- Circuit breaking.
- Request correlation IDs.
- Response transformation.
- Metrics and logging.
Architecture
Client
  |
  v
Gateway
  |
  +---- Authentication
  |
  +---- Rate Limiter
  |
  +---- Routing
  |
  +---- Timeout / Circuit Breaker
  |
  +---- Service A
  |
  +---- Service B

Compare fixed-window, sliding-window, and token-bucket rate limiting. Document which algorithms you implement and why.

Measure throughput and latency under controlled load. Include a clear account of the test environment; don't present results from a laptop as proof of production-scale capacity.