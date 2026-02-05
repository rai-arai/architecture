# Arai Architecture

Welcome! This repository is where architectural decisions for
[Arai](https://gitlab.com/rai.onl/arai) are proposed, discussed, and recorded.

## What is Arai?

Arai is a self-sovereign agent management platform built in Rust with
WebAssembly-based extensibility. It provides a standards-compliant runtime and
orchestration platform for executing, coordinating, and governing AI agents —
from edge devices to sovereign clouds. Arai implements AAIF open standards (MCP,
A2A) as native architectural primitives, enabling interoperability with any
compliant agent platform.

## What this repository is for

This repository tracks architectural decisions using two complementary
approaches:

- **Architecture decision records (ADRs)** capture internal technical and
  organisational decisions — how Arai is built, structured, and maintained.

- **Requests for comments (RFCs)** handle community-facing proposals — changes
  to public interfaces, features, behaviour, and integration patterns that
  affect how people use Arai.

Both approaches are open to everyone. You don't need to be a maintainer or a
regular contributor to submit a proposal. If you have an idea or see something
that could be improved, you're welcome here.

## How the process works

1. **Create an issue** using one of the issue templates (ADR or RFC) to signal
   your intent and invite early feedback.
2. **Draft a proposal** using the document templates in `templates/`.
3. **Submit a merge request** with your proposal in `adrs/` or `rfcs/`.
4. **Discuss** — for ADRs, technical leads review over 7–14 days. For RFCs, the
   community discusses for a minimum of 14 days.
5. **Decision** — once consensus is reached, the proposal is merged and becomes
   part of the project's record.

The full process, including how consensus works, how disagreements are resolved,
and what happens with urgent decisions, is documented in the
[Omnifi Foundation handbook](https://handbook.omnifi.coop/engineering/architecture/).

## Projects in scope

Proposals in this repository may affect any part of the Arai ecosystem:

**Runtime**
- Agent execution engine and Wasm sandbox
- Agent memory and state persistence
- Platform adapters

**Orchestration**
- Agent coordination and lifecycle management
- Task delegation and workflow execution

**Protocol libraries**
- MCP client and server implementations
- A2A protocol implementation

**Knowledge layer**
- MCP server connectors for enterprise data sources
- Knowledge graph engine
- Privacy-preserving federation

**Plugin SDK and tooling**
- Rust SDK for plugin authors
- CLI for plugin development workflow
- Wasm compilation and validation tooling

**Platform targets**
- Fastly Compute, bare metal, containers, Kubernetes

**Ecosystem integrations**
- Rai Shield integration (AI model traffic routing and governance)
- Prism integration (federated learning)
- Rai LS integration (content licensing)

If your proposal spans multiple areas, note all affected projects in your
proposal so the right people can weigh in.

## Governance

Arai is governed by the [Omnifi Foundation](https://omnifi.coop), a
community-driven organisation that stewards open source projects. The
architecture decision process — how proposals are written, reviewed, and
decided — is defined in the
[Omnifi Foundation handbook](https://handbook.omnifi.coop/engineering/architecture/)
and applies equally to all contributors.

[Responsible Engineering Ab](https://responsible.engineering) is a contributing
organisation that develops Arai and distributes commercial builds of the
software. All code is contributed to the foundation and governed through this
open process.

Decisions are made through consensus. Technical leads facilitate the process but
don't dictate outcomes. Every voice carries weight, and dissenting perspectives
are documented and valued. See the
[governance model](https://handbook.omnifi.coop/engineering/architecture/governance/)
for full details.

## Getting started

New to the project? Here's how to get oriented:

1. **Browse existing proposals** in `adrs/` and `rfcs/` to see what's been
   decided and how proposals are structured.
2. **Check open merge requests** for proposals currently under discussion.
3. **Read the handbook** for
   [detailed process guidance](https://handbook.omnifi.coop/engineering/architecture/).
4. **Open an issue** if you have questions — there are no bad questions.

## Repository structure

```
├── README.md              You are here
├── CONTRIBUTING.md        How to submit proposals
├── templates/
│   ├── adr.md             Architecture decision record template
│   └── rfc.md             Request for comments template
├── adrs/                  Accepted architecture decision records
├── rfcs/                  Accepted requests for comments
└── .gitlab/
    └── issue_templates/
        ├── adr.md         Issue template for starting an ADR
        └── rfc.md         Issue template for starting an RFC
```

## Code of conduct

All participation is subject to the
[Omnifi Foundation code of conduct](https://handbook.omnifi.coop/CODE_OF_CONDUCT/).
We're committed to a welcoming, respectful, and inclusive environment.

## License

CC BY-SA 4.0 — see LICENSE for details.
