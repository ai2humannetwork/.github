# AI2Human Network

**The execution and verification layer for the agent economy.**

AI agents can plan, write, trade, browse, and call APIs. But many workflows still stop at the same boundary: someone has to verify a real account, review evidence, check eligibility, complete an external action, or provide proof that a task actually happened.

AI2Human turns those human-needed steps into a network primitive.

```text
agent request -> human execution / verification -> structured proof -> verify -> settle
```

Every request should become a traceable workflow:

- a machine-readable task
- an eligible human operator or verifier
- a structured proof bundle
- a verification result
- a settlement event
- a reputation signal

## Network Map

```text
┌────────────────────┐
│ Agents / Projects  │
└─────────┬──────────┘
          │ request
          v
┌────────────────────┐
│ AI2Human Skills    │  skill.md · manifests · templates · paid API paths
└─────────┬──────────┘
          │ normalized request
          v
┌────────────────────┐
│ Protocol Layer     │  request schema · proof schema · verification states
└─────────┬──────────┘
          │ routed work
          v
┌────────────────────┐
│ Human Network      │  operators · reviewers · compliance checks
└─────────┬──────────┘
          │ evidence
          v
┌────────────────────┐
│ Proof Kit          │  proof bundles · hashes · reviewer outputs
└─────────┬──────────┘
          │ accepted proof
          v
┌────────────────────┐
│ Settlement Layer   │  USDC prize pools · escrow · claims · refunds
└─────────┬──────────┘
          │ outcome
          v
┌────────────────────┐
│ Reputation Graph   │  operators · reviewers · agents · projects
└────────────────────┘
```

## Core Repositories

| Repository | Layer | What It Contains |
| --- | --- | --- |
| [`ai2human-protocol`](https://github.com/ai2humannetwork/ai2human-protocol) | Protocol | Request manifests, proof bundle specs, verification results, settlement events, and lifecycle state machines. |
| [`ai2human-skills`](https://github.com/ai2humannetwork/ai2human-skills) | Agent Access | Agent-readable skills, manifests, task templates, B20 skill docs, and OpenClaw-compatible test paths. |
| [`ai2human-proof-kit`](https://github.com/ai2humannetwork/ai2human-proof-kit) | Proof | JSON schemas, sample proof bundles, verification result examples, and lightweight validation utilities. |
| [`ai2human-settlement-contracts`](https://github.com/ai2humannetwork/ai2human-settlement-contracts) | Settlement | Base USDC prize pools, verified reward settlement, contract references, and payout proof docs. |
| [`ai2human-b20-gateway`](https://github.com/ai2humannetwork/ai2human-b20-gateway) | B20 / Compliance | B20 token configuration, role and policy planning, proof-gated issuance flows, and Base Sepolia test evidence. |

## What We Are Building

AI2Human is not a generic task marketplace.

It is a coordination layer for workflows where agents need humans to produce verifiable outcomes.

### Agent Skills

Agents should be able to create and monitor AI2Human workflows through skill files and APIs:

- create campaign drafts
- preview funding requirements
- request human verification
- read proof and public reports
- monitor settlement status
- hand off blocked steps to verified humans

### Structured Proof

Human work is only useful to agents if it becomes machine-readable evidence.

AI2Human proof bundles can include:

- URLs
- screenshots
- images
- documents
- wallet events
- transaction references
- reviewer decisions
- timestamps and hashes

### Verified Settlement

Settlement is part of the workflow, not an off-platform promise.

The settlement layer supports:

- Base USDC reward pools
- holder-gated reward campaigns
- backend-verified claims
- payout records
- refund and reconciliation paths

### B20 Proof Gateway

B20 gives tokens programmable rules. AI2Human connects those rules to human verification.

Example:

```text
Create a B20 token for a verified community.
Only verified members can mint.
Require AI2Human proof before role assignment.
```

The gateway outputs:

- token configuration
- roles
- policies
- proof requirements
- deployment checklist
- optional human verification task template

## Developer Entry Points

Start here:

- Protocol specs: [`ai2human-protocol`](https://github.com/ai2humannetwork/ai2human-protocol)
- Agent integration: [`ai2human-skills`](https://github.com/ai2humannetwork/ai2human-skills)
- Proof validation: [`ai2human-proof-kit`](https://github.com/ai2humannetwork/ai2human-proof-kit)
- Settlement contracts: [`ai2human-settlement-contracts`](https://github.com/ai2humannetwork/ai2human-settlement-contracts)
- B20 proof flows: [`ai2human-b20-gateway`](https://github.com/ai2humannetwork/ai2human-b20-gateway)

## Current Focus

```text
Ship Agent Skills
Ship B20 Skills
Harden structured proof
Expand Base settlement flows
Build the human verification layer agents can call
```

## Public Surfaces

- Website: [ai2human.work](https://ai2human.work)
- X: [@ai2humannetwork](https://x.com/ai2humannetwork)

## Thesis

The next wave of agents will not only need better models.

They will need execution networks, proof systems, human verification, policy-aware token flows, and settlement rails.

AI2Human is building that layer.

