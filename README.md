# BitFury

Bitfury Group is a blockchain technology company founded in 2011 as one of the earliest Bitcoin mining hardware makers and full-cycle infrastructure providers, and now operating as a technology incubator headquartered in London. Its developer-facing surface is **Exonum**, the open-source (Apache-2.0) framework Bitfury Group Limited built for private and permissioned blockchain applications.

- Company: https://bitfury.com/
- Exonum: https://exonum.com/ — docs at https://exonum.com/doc/version/latest/
- Source: https://github.com/exonum
- Secondary market listing: https://forgeglobal.com/bitfury-group_stock/

## What is in this repo

| Directory | What it holds |
|---|---|
| `grpc/` | The Exonum Protobuf message definitions, saved verbatim from `exonum/exonum-proto-sources` |
| `packages/` | Verified Rust, JavaScript, Python and Java packages published by the Exonum team |
| `cli/` | The `exonum-cli` node management command surface |
| `sandbox/` | The testkit and `run-dev` local development surface (no hosted sandbox exists) |
| `authentication/` | The Ed25519-signature / public-vs-private-server authorization model |
| `conventions/` | Endpoint layout, pagination, consistency model, error envelope, proofs |
| `errors/` | The `ExecutionError` envelope plus the full core and common error code lists |
| `data-model/` | Entity graph derived from the Protobuf definitions |
| `asyncapi/` | The explorer WebSocket pub/sub event surface (no AsyncAPI document is published) |
| `lifecycle/`, `changelog/` | Versioning, deprecation guidance, release history |
| `conformance/`, `security/`, `well-known/` | Standards posture and probe records |
| `llms/` | Generated `llms.txt` for agents |

## Notes

Exonum is **self-hosted software, not a hosted API** — there is no vendor base URL, signup, API key or sandbox tenant. Bitfury publishes no OpenAPI, GraphQL, AsyncAPI or MCP definition, no `/.well-known/` documents and no A2A agent card; none were authored on its behalf. The last Exonum release is 1.0.0 (2020-03-31).
