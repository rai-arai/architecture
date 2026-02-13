# Decision

<!--
Use this template to propose technical and organisational decisions for Arai.
Decisions are also known as architecture decision records (ADRs).
For community-facing changes, use the comment template instead.

After creating this issue, draft your full proposal using the template at
templates/decision.md and submit a merge request.

Process details: https://handbook.omnifi.coop/engineering/architecture/governance/
-->

## Overview

### Title
<!-- A clear, descriptive title for the decision -->

### Affected projects
<!-- Which Arai projects does this decision affect? -->
- [ ] Runtime (execution engine, Wasm sandbox, plugin loading, agent memory)
- [ ] Orchestration (agent coordination, lifecycle management, task delegation)
- [ ] Protocol libraries (MCP client/server, A2A implementation)
- [ ] Knowledge layer (MCP server connectors, knowledge graph engine, federation)
- [ ] Platform targets (Fastly Compute, bare metal, containers, Kubernetes)
- [ ] Plugin SDK and tooling (SDK for plugin authors, CLI tools)
- [ ] Ecosystem integrations (Shield, Prism, Rai LS)
- [ ] Other: <!-- specify -->

---

## Problem statement

### Current situation
<!-- Describe the technical or organisational situation requiring this decision -->

### Decision drivers
<!-- What factors are influencing this decision? -->
- <!-- Driver 1 -->
- <!-- Driver 2 -->
- <!-- Driver 3 -->

---

## Proposed decision

### Chosen approach
<!-- State the proposed decision clearly -->

### Rationale
<!-- Why is this approach being proposed? -->

### Alternatives considered
<!-- Briefly list other approaches you considered -->

---

## Impact summary

### Technical impact
<!-- How does this affect the codebase and architecture? -->

### Contributor impact
<!-- How does this affect how people contribute to the project? -->

---

## Next steps

- [ ] Draft full proposal in `decisions/XXXX-title.md`
- [ ] Submit merge request for review
- [ ] Address feedback from technical leads
- [ ] Update status after decision

---

## Governance

This decision follows the
[Omnifi Foundation governance model](https://handbook.omnifi.coop/engineering/architecture/governance/).
Technical leads carry responsibility for shepherding proposals through the
process. See the
[handbook](https://handbook.omnifi.coop/engineering/architecture/governance/) for
process details.

/label ~"decision" ~"architecture"
