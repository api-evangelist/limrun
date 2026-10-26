# Limrun

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
