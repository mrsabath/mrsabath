# Mariusz Sabath

**Senior Technical Staff Member, AI Platform** | IBM Research
[SPIFFE Steering Committee](https://github.com/spiffe/spiffe/blob/main/ssc/README.md) member · Co-creator of [Tornjak](https://github.com/spiffe/tornjak) (CNCF)

Building zero-trust identity and platform primitives for cloud-native AI agents.

[![Website](https://img.shields.io/badge/Website-mrsabath.github.io-2ea44f?style=flat&logo=github&logoColor=white)](https://mrsabath.github.io)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-mariusz--sabath-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mariusz-sabath-b36b0b20/)
[![X](https://img.shields.io/badge/X-@mrsabath-000000?style=flat&logo=x&logoColor=white)](https://x.com/mrsabath)
[![rossoctl](https://img.shields.io/badge/project-rossoctl.dev-D32F2F?style=flat&logo=kubernetes&logoColor=white)](https://www.rossoctl.dev/)

---

## Current Focus

When AI agents act on behalf of users — committing code, calling APIs, triggering workflows — who holds the identity?

I work on **[rossoctl](https://www.rossoctl.dev/)** (formerly *Kagenti*): open-source platform primitives for
trustworthy AI agents on Kubernetes. It is framework-neutral, built on open standards, and supports
[A2A](https://a2a-protocol.org/latest/) and [MCP](https://modelcontextprotocol.io/).

My focus is the security and identity layer: [SPIFFE/SPIRE](https://spiffe.io/) workload identity,
OAuth 2.0 token exchange ([RFC 8693](https://datatracker.ietf.org/doc/html/rfc8693)), and transparent
sidecar injection — so agent developers never write auth code.

```
  User                 Agent                 Token Exchange              Target Service
(authorization) ──▶ (SPIFFE identity) ──▶     (RFC 8693)       ──▶    (scoped access)
                           │                       │
                   zero code changes      subject preserved → audit trail
```

The agent holds cryptographic identity. The user holds delegated authorization. The platform enforces policy.

## Key Projects

| Project | Role | Description |
|---|---|---|
| [rossoctl/rossoctl](https://github.com/rossoctl/rossoctl) | Creator & Maintainer | Agentic platform — installer, UI, and docs for running secure AI agents on Kubernetes |
| [rossoctl/cortex](https://github.com/rossoctl/cortex) | Creator & Maintainer | Data plane that mediates agent actions — admission webhook, AuthBridge, client registration |
| [rossoctl/operator](https://github.com/rossoctl/operator) | Maintainer | Kubernetes operator for deploying and managing the lifecycle of Agents and Tools |
| [rossoctl/examples](https://github.com/rossoctl/examples) | Creator & Maintainer | Reference agent implementations and demo tools |
| [rossoctl/.github](https://github.com/rossoctl/.github) | Creator & Maintainer | Project website and org-level community health files — [rossoctl.dev](https://www.rossoctl.dev/) |
| [spiffe/tornjak](https://github.com/spiffe/tornjak) | Co-creator & Maintainer | SPIRE management UI and API layer (CNCF) |
| [Kuadrant/mcp-gateway](https://github.com/Kuadrant/mcp-gateway) | Contributor | Envoy-based MCP Gateway with Istio and policy attachment integration |

> `kagenti/*` repositories were renamed to [`rossoctl/*`](https://github.com/rossoctl) — old links redirect.

## Technical Interests

- **Workload Identity** — SPIFFE/SPIRE, JWT-SVIDs, attestation, chain-of-trust
- **Agent Security** — OAuth 2.0 token exchange, subject preservation, scope-based access control
- **Agent Attestation** — stackable attestors enriching identity with provenance, capabilities, and SBOM verification
- **Cloud-Native Infrastructure** — Kubernetes admission webhooks, Envoy sidecars, service mesh coexistence

## Speaking

- **KubeCon + CloudNativeCon Europe 2026** — *When an Agent Acts on Your Behalf, Who Holds the Keys?*
  Cryptographic identity and delegation for cloud-native AI agents
- Full talk list with recordings on [mrsabath.github.io](https://mrsabath.github.io)

## Writing

- **[rossoctl.dev](https://www.rossoctl.dev/)** — project site: architecture, docs, blog, and getting-started guides
- **[Publications & patents](https://mrsabath.github.io)** — NIST IR 8320B, Red Hat and IBM Research articles, 20 patents

## GitHub Activity

<a href="https://github.com/mrsabath">
  <img src="https://github-readme-stats.vercel.app/api?username=mrsabath&show_icons=true&hide_border=true&count_private=true" alt="GitHub stats for mrsabath" height="170" />
</a>

---

**Ask me about:** SPIFFE/SPIRE · zero-trust for AI agents · Kubernetes workload identity
**Contact:** mrsabath _at_ gmail.com
