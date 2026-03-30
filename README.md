# Mariusz Sabath

**Senior Technical Staff Member** | IBM Research, Hybrid Cloud
[SPIFFE Steering Committee](https://github.com/spiffe/spiffe/blob/main/ssc/README.md) Member | Building zero-trust identity infrastructure for cloud-native AI agents

[![LinkedIn](https://img.shields.io/badge/LinkedIn-mariusz--sabath-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://linkedin.com/in/mariusz-sabath-b36b0b20)
[![Web](https://img.shields.io/badge/Web-mrsabath.github.io-2ea44f?style=flat&logo=github)](https://mrsabath.github.io)
[![X](https://img.shields.io/badge/X-@mrsabath-000000?style=flat&logo=x&logoColor=white)](https://x.com/mrsabath)

---

## Current Focus

When AI agents act on behalf of users -- committing code, calling APIs, triggering workflows -- who holds the identity?

I'm building **[Kagenti](https://kagenti.github.io/.github/)** -- an open-source platform for deploying, securing, and governing AI agents on Kubernetes. The security layer uses SPIFFE/SPIRE, OAuth 2.0 token exchange ([RFC 8693](https://datatracker.ietf.org/doc/html/rfc8693)), and transparent sidecar injection so agent developers never write auth code.

```
User (authorization) --> Agent (SPIFFE identity) --> Token Exchange (RFC 8693) --> Target Service
                          |                               |
                     Zero code changes              Subject preserved (audit trail)
```

The agent holds cryptographic identity. The user holds delegated authorization. The platform enforces policy.

## Recent Talks

- **KubeCon + CloudNativeCon Europe 2026** -- *"When an Agent Acts on Your Behalf, Who Holds the Keys?"* -- Cryptographic identity and delegation for cloud-native AI agents

## Key Projects

| Project | Role | Description |
|---------|------|-------------|
| [kagenti/kagenti](https://github.com/kagenti/kagenti) | Creator & Maintainer | Agentic platform -- installer, UI, orchestration for secure AI agents on Kubernetes |
| [kagenti/kagenti-extensions](https://github.com/kagenti/kagenti-extensions) | Creator & Maintainer | Admission webhook, AuthBridge (AuthProxy + client registration), Helm charts |
| [kagenti/agent-examples](https://github.com/kagenti/agent-examples) | Creator & Maintainer | Reference agent implementations and demo tools |
| [spiffe/tornjak](https://github.com/spiffe/tornjak) | Co-creator & Maintainer | SPIRE management UI and API layer (CNCF) |
| [Kuadrant/mcp-gateway](https://github.com/Kuadrant/mcp-gateway) | Contributor | Envoy-based MCP Gateway with Istio and policy attachment integration |

## Technical Interests

- **Workload Identity** -- SPIFFE/SPIRE, JWT-SVIDs, attestation, chain-of-trust
- **Agent Security** -- OAuth 2.0 token exchange, subject preservation, scope-based access control
- **Cloud-Native Infrastructure** -- Kubernetes admission webhooks, Envoy sidecars, service mesh coexistence
- **Agent Attestation** -- Stackable attestors enriching identity with agent provenance, capabilities, and SBOM verification

## Writing

- [Kagenti Blog](https://medium.com/kagenti-the-agentic-platform) -- Technical deep-dives on agent identity, AuthBridge architecture, and zero-trust patterns
- [kagenti.io](https://kagenti.github.io/.github/) -- Project site, architecture, and getting-started guides

## GitHub Activity

<a href="https://github.com/mrsabath">
  <img src="https://github-readme-stats.vercel.app/api?username=mrsabath&show_icons=true&hide_border=true&count_private=true" alt="GitHub Stats" height="180" />
</a>

<a href="https://github.com/mrsabath">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=mrsabath&theme=default" alt="Contribution Graph" />
</a>

<p>
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=mrsabath&theme=default" alt="Stats" height="180" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=mrsabath&theme=default&utcOffset=-4" alt="Productive Time" height="180" />
</p>

---

**Contact:** mrsabath _at_ gmail.com | **Ask me about:** SPIFFE/SPIRE, zero-trust for AI agents, Kubernetes workload identity
