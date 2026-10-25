<div align="center">

<img src="https://raw.githubusercontent.com/hump-cdc/hump/main/apps/hump-tower/public/logo_lg.svg" width="120" alt="Hump logo">

<h1>Hump</h1>

<p>Your database, as an event stream.</p>

[Website](https://hump.dev) · [Documentation](https://hump.dev/docs/getting-started) · [Releases](https://github.com/hump-cdc/hump/releases) · [Docker Hub](https://hub.docker.com/r/humpcdc/hump)

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/hump-cdc/hump/blob/main/LICENSE)
[![OpenSSF Scorecard](https://api.scorecard.dev/projects/github.com/hump-cdc/hump/badge)](https://scorecard.dev/viewer/?uri=github.com/hump-cdc/hump)
[![OpenSSF Best Practices](https://www.bestpractices.dev/projects/15877/badge)](https://www.bestpractices.dev/projects/15877)
[![SLSA 3](https://slsa.dev/images/gh-badge-level3.svg)](https://github.com/hump-cdc/hump#verifying-the-image)

</div>

In a microservice system each service owns its database, and other services still need to know what changed in it. Hump reads every insert, update, delete and truncate from PostgreSQL logical replication and publishes each change as an event to Kafka, NATS, RabbitMQ or HTTP webhooks.

It uses the built-in `pgoutput` plugin, so PostgreSQL needs no extensions. The service doesn't need an outbox table, dual writes or event-publishing code. Hump is MIT-licensed.

## Repositories

| Repository | Description |
|---|---|
| [hump](https://github.com/hump-cdc/hump) | The CDC service: PostgreSQL to Kafka, NATS, RabbitMQ and webhooks. |
| [benchmarks](https://github.com/hump-cdc/benchmarks) | Performance benchmarks. |

## Supply chain

Release images are signed with keyless cosign and ship with SLSA build provenance and an SPDX SBOM. See [Verifying the image](https://github.com/hump-cdc/hump#verifying-the-image) for how to check them.

## Contributing

Read [CONTRIBUTING.md](https://github.com/hump-cdc/hump/blob/main/CONTRIBUTING.md) before opening a pull request. Report bugs in [Issues](https://github.com/hump-cdc/hump/issues) and discuss ideas in [Discussions](https://github.com/hump-cdc/hump/discussions).

---

Questions go to [Discussions](https://github.com/hump-cdc/hump/discussions). Report vulnerabilities privately through the [advisory form](https://github.com/hump-cdc/hump/security/advisories/new), not in public issues.

Hump is released under the MIT License. Website: [hump.dev](https://hump.dev).
