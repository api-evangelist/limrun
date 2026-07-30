# Limrun

Limrun (Limrun, Inc.) is a Y Combinator-backed cloud infrastructure company for mobile development.
It exists so cloud coding agents and Linux CI runners can build, run, and test iOS and Android apps
without a Mac: iOS simulators on real Macs, remote Xcode and Bazel build sandboxes, accelerated
Android emulators over an ADB tunnel, Gradle build sandboxes, and a managed Asset Storage service —
all behind one REST control plane at `api.limrun.com`.

- Website: https://lim.run
- Docs: https://docs.limrun.com/docs
- API reference: https://docs.limrun.com/docs/reference/sdk
- Console: https://console.limrun.com
- Status: https://status.limrun.com
- GitHub: https://github.com/limrun-inc

Backed by: y-combinator

## What makes this provider notable

Every instance returns its own per-instance Model Context Protocol server (`status.mcpUrl`) alongside
its data-plane URLs — a per-instance MCP endpoint rather than one shared server. Limrun also
publishes five first-party Agent Skills with a `catalog.json` manifest and a CI validator, which
places it among the small set of providers shipping agent-native surfaces as products rather than
as documentation.

## Artifacts

| Artifact | Path | Method |
|---|---|---|
| OpenAPI 3.0 (26 ops, 35 schemas) | `openapi/limrun-openapi-original.yml` | searched |
| OpenAPI Overlay | `overlays/limrun-api-overlay.yaml` | generated |
| llms.txt | `llms/limrun-llms.txt` | searched |
| Agent Skills (5, verbatim) | `skills/` | searched |
| MCP server | `mcp/limrun-mcp.yml` | searched |
| Packages / SDKs | `packages/limrun-packages.yml` | searched |
| CLI (`lim`) | `cli/limrun-cli.yml` | searched |
| Embedded components (`@limrun/ui`) | `components/limrun-components.yml` | searched |
| Authentication | `authentication/limrun-authentication.yml` | searched |
| OAuth scopes (MCP) | `scopes/limrun-scopes.yml` | searched |
| Well-known | `well-known/limrun-well-known.yml` | searched |
| Conventions + idempotency | `conventions/limrun-conventions.yml` | searched |
| Error catalog | `errors/limrun-problem-types.yml` | searched |
| Lifecycle + status page | `lifecycle/limrun-lifecycle.yml` | searched |
| Changelog | `changelog/limrun-changelog.yml` | searched |
| Sandbox / console | `sandbox/limrun-sandbox.yml` | searched |
| Conformance | `conformance/limrun-conformance.yml` | derived |
| Data model | `data-model/limrun-data-model.yml` | derived |
| Agentic access | `agentic-access/limrun-agentic-access.yml` | generated |
| Domain security | `security/limrun-domain-security.yml` | probed |
| Vulnerability disclosure | `security/limrun-vulnerability-disclosure.yml` | searched |

## Gaps observed

Limrun is in Early Access, and the commercial and trust surface reflects that. Not published as of
2026-07-19: pricing, terms of service, privacy policy, blog, roadmap, `/.well-known/security.txt`,
a responsible-disclosure page, a trust center or any compliance certification, a deprecation or
versioning policy, an SLA, and any webhook or event surface (so no AsyncAPI applies). The published
OpenAPI also omits `servers`, `securitySchemes`, tags, and non-2xx responses that the SDK reference
documents in prose — captured in `overlays/limrun-api-overlay.yaml`.
