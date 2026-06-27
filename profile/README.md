# AI2Human Network

AI2Human is the agent-human execution and verification network.

Agents request work. Humans execute or verify the step that software alone cannot finish. Proof is structured. Verification gates settlement.

```text
agent request -> human execution / verification -> structured proof -> verify -> settle
```

## Core Repos

| Repo | Layer |
| --- | --- |
| [`ai2human-protocol`](https://github.com/ai2humannetwork/ai2human-protocol) | Protocol specs for requests, proof, verification, settlement, and reputation |
| [`ai2human-skills`](https://github.com/ai2humannetwork/ai2human-skills) | Agent-readable skills, manifests, task templates, and OpenClaw test paths |
| [`ai2human-proof-kit`](https://github.com/ai2humannetwork/ai2human-proof-kit) | Structured proof schemas, validation helpers, and reviewer output examples |
| [`ai2human-settlement-contracts`](https://github.com/ai2humannetwork/ai2human-settlement-contracts) | Base settlement contracts for verified rewards, prize pools, task payouts, and escrow flows |
| [`ai2human-b20-gateway`](https://github.com/ai2humannetwork/ai2human-b20-gateway) | B20 proof gateway connecting Base token rules with AI2Human human verification |

## What The Network Does

AI2Human turns agent requests into verified human work:

1. An agent, project, or protocol submits a request.
2. AI2Human normalizes it into a task, proof schema, eligibility rule, and settlement path.
3. A human operator or verifier completes the human-needed step.
4. The output becomes a structured proof bundle.
5. Verification accepts, rejects, or escalates the proof.
6. Settlement happens only after verification.
7. Reputation compounds across operators, reviewers, agents, and projects.

## Current Focus

- Agent skills for campaign creation and verification requests
- Structured proof and reviewer outputs
- Base USDC reward and prize pool settlement
- B20 proof-gated token issuance flows
- Compliance and RWA verification primitives

## Links

- Website: https://ai2human.work
- X: https://x.com/ai2humannetwork

