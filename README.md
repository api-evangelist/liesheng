# Liesheng Group

Liesheng Group (猎声集团 / Liesheng Technology) is a Dongguan, Guangdong consumer-electronics company founded on 25 May 2015 as one of Xiaomi's first ecosystem-chain suppliers. It operates as a global ODM/OEM solution provider — it engineered the Redmi AirDots true-wireless earbuds — while building its own brand portfolio, reaching more than 100 countries and regions.

- **HAYLOU** — wireless audio, smart wearables, bone-conduction headphones and microphones; brand launched 2017.
- **SUUNTO** — the 85-year-old Finnish premium sports-watch and outdoor-instrument brand, acquired by Liesheng in 2022.

## Developer surface

Liesheng publishes no corporate API. Two real surfaces exist in the estate:

- **[Suunto Cloud API](https://apizone.suunto.com/apis)** — partner-gated OAuth2 access to a Suunto App user's workouts (FIT files with GPS tracks and sensor samples) and daily activity, plus workout and route push. Base URL `https://cloudapi.suunto.com`, version `v2`. Free of charge, but access requires acceptance into the [Suunto partner program](https://www.suunto.com/welcomepartners) and a signed API agreement; personal use is not offered. Webhooks announce new workouts. No OpenAPI, no SDK.
- **[HAYLOU Commerce (UCP/MCP)](https://haylou.com/agents.md)** — a live Universal Commerce Protocol MCP endpoint at `https://haylou.com/api/ucp/mcp` for agent-driven shopping, provisioned by Shopify and served from the haylou.com origin.

## Artifacts

| Artifact | File |
|---|---|
| Authentication | `authentication/liesheng-authentication.yml` |
| OAuth scopes | `scopes/liesheng-scopes.yml` |
| Conventions | `conventions/liesheng-conventions.yml` |
| Webhooks | `asyncapi/liesheng-suunto-webhooks.yml` |
| MCP server | `mcp/liesheng-mcp.yml` |
| Sandbox / testing | `sandbox/liesheng-sandbox.yml` |
| Lifecycle | `lifecycle/liesheng-lifecycle.yml` |
| Conformance | `conformance/liesheng-conformance.yml` |
| Well-known index | `well-known/liesheng-well-known.yml` |
| Packages | `packages/liesheng-packages.yml` |
| llms.txt | `llms/liesheng-llms.txt` |
| Domain security | `security/liesheng-domain-security.yml` |

## Notes

- No OpenAPI, AsyncAPI or Protobuf is published, so no spec, error catalog, data model, overlay or agent skill has been derived — nothing has been fabricated to fill those slots.
- No first-party SDK exists in any language; the API Zone FAQ states there is no mobile SDK.
- No status page, dated changelog, published roadmap, vulnerability-disclosure program or trust center was found.
- `https://liesheng.cc` serves an expired certificate issued for `www.haylou.cn` (expired 2025-12-09) — hostname mismatch and expiry both fail verification.

Backed by: qiming — https://liesheng.cc
