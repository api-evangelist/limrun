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

Limrun (Limrun, Inc.) is a Y Combinator-backed cloud infrastructure company for mobile development, built so cloud coding agents and Linux CI runners can build, run, and test iOS and Android apps without a Mac. Limrun exposes three composable cloud services behind one REST control plane at api.limrun.com: iOS simulators running on real Macs (streamable in a browser and drivable programmatically through taps, screenshots, accessibility element trees, video recording, and app lifecycle), remote Xcode and Bazel build sandboxes that accept synced sources and run xcodebuild or remote build execution, and accelerated Android emulators reachable over an ADB tunnel by Android Studio, Appium, or scrcpy. Gradle build sandboxes and a managed Asset Storage service for .apk and .app build artifacts round out the platform. Every instance is created through the control plane with an org API key and returns its own per-instance token, data-plane URLs, a signed browser stream URL, and its own Model Context Protocol server, which makes Limrun one of the few providers shipping a per-instance MCP endpoint alongside first-party Agent Skills for coding agents.

**Areas:** Company · Mobile · iOS · Android · Simulator · Emulators · Cloud Infrastructure · Continuous Integration · Developer Tools · Testing · Agents · MCP

## Limrun on APIs.io

Everything profiled for Limrun is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/limrun/](https://apis.io/providers/limrun/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Limrun Analytics API](https://apis.io/apis/limrun/limrun-analytics-api/) — The Analytics API from Limrun — 3 operation(s) for analytics.
- [Limrun Android Instances API](https://apis.io/apis/limrun/limrun-android-instances-api/) — The Android Instances API from Limrun — 2 operation(s) for android instances.
- [Limrun Assets API](https://apis.io/apis/limrun/limrun-assets-api/) — The Assets API from Limrun — 2 operation(s) for assets.
- [Limrun Downloads API](https://apis.io/apis/limrun/limrun-downloads-api/) — The Downloads API from Limrun — 1 operation(s) for downloads.
- [Limrun Gradle Instances API](https://apis.io/apis/limrun/limrun-gradle-instances-api/) — The Gradle Instances API from Limrun — 2 operation(s) for gradle instances.
- [Limrun Ios Instances API](https://apis.io/apis/limrun/limrun-ios-instances-api/) — The Ios Instances API from Limrun — 2 operation(s) for ios instances.
- [Limrun Xcode Instances API](https://apis.io/apis/limrun/limrun-xcode-instances-api/) — The Xcode Instances API from Limrun — 4 operation(s) for xcode instances.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [limrun-instance](https://apis.io/servers/limrun/limrun-instance/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Limrun Agentic Access](https://apis.io/agentic-access/limrun/limrun-agentic-access/)

#### Collections (7)

Postman and Open Collection request collections.

- [Limrun Analytics API](https://apis.io/collections/limrun/open-limrun-analytics-api/)
- [Limrun Analytics Android Instances API](https://apis.io/collections/limrun/open-limrun-android-instances-api/)
- [Limrun Analytics Assets API](https://apis.io/collections/limrun/open-limrun-assets-api/)
- [Limrun Analytics Downloads API](https://apis.io/collections/limrun/open-limrun-downloads-api/)
- [Limrun Analytics Gradle Instances API](https://apis.io/collections/limrun/open-limrun-gradle-instances-api/)
- [Limrun Analytics Ios Instances API](https://apis.io/collections/limrun/open-limrun-ios-instances-api/)
- [Limrun Analytics Xcode Instances API](https://apis.io/collections/limrun/open-limrun-xcode-instances-api/)

#### Overlays (1)

OpenAPI overlays, including conversational phrasing for each operation.

- [Limrun Api Overlay](https://apis.io/overlays/limrun/limrun-api-overlay/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Limrun Authentication](https://apis.io/security/limrun/limrun-authentication/)
- [Limrun Domain Security](https://apis.io/security/limrun/limrun-domain-security/)
- [Limrun Vulnerability Disclosure](https://apis.io/security/limrun/limrun-vulnerability-disclosure/)

#### OAuth scopes (1)

The permissions the API asks for.

- [Limrun Scopes](https://apis.io/scopes/limrun/limrun-scopes/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://lim.run)
- [Documentation](https://docs.limrun.com/docs)
- [Getting started](https://docs.limrun.com/docs/quickstart)
- [API reference](https://docs.limrun.com/docs/reference/sdk)
- [Sign up](https://console.limrun.com)
- [Security](https://github.com/limrun-inc/typescript-sdk/blob/main/SECURITY.md)
- [GitHub](https://github.com/limrun-inc)
- [Status](https://status.limrun.com)

## API Evangelist rating

**Kin Score 38.2** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 71.7 |
| Contract quality | 34.5 |
| Contract governance | 4.5 |
| Operational transparency | 36.8 |
| Developer ergonomics | 76.2 |
| Access clarity | 0.0 |

**Agent readiness 43.0** — agent-native

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | documented (partial credit) |
| Auth Clarity | served (partial credit) |
| Idempotency | documented (partial credit) |
| Error Semantics | documented (partial credit) |
| OpenAPI Examples | — |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | yes |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | — |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |

**Regulatory alignment 32.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/limrun/](https://apis.io/providers/limrun/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Limrun: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/limrun/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
