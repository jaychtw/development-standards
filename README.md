# Game Development Standards

Central, versioned guidance for AI-assisted games and application projects.

## Governing documents

- [UGDS v1.0.0](UGDS.md) — adopted **game development quality** baseline. Pin the precise UGDS tag or commit in each adopting project; existing projects are not retroactively certified.
- [AI Collaboration & Continuity Protocol (AICP) v1.3.0](AI-COLLABORATION-PROTOCOL.md) — shared AI/human collaboration, memory recovery, decisions, evidence, handoffs and approval boundaries. Applies to games and apps that adopt it.

## Templates

- [GDD](templates/GDD-TEMPLATE.md) — project gameplay/experience and rules.
- [Codex brief](templates/CODEX-BRIEF.md) — bounded implementation assignment.
- [Project state](templates/PROJECT_STATE.md) — lightweight current-state index in each project's repo.
- [Conversation starter](templates/CONVERSATION-STARTER.md) — reusable opening message for a new ChatGPT Game Development conversation.

## Routine Possibility publication

At project closure, the **individual game/app conversation** coordinates its Possibility catalog handoff after an independently verified release; the Possibility workstream handles shared platform changes. Publication remains a distinct, authorization-gated step. See [AICP §10](AI-COLLABORATION-PROTOCOL.md) and the portal's [catalog contract](https://github.com/jaychtw/jaychtw.github.io/blob/main/docs/CATALOG.md).

## Continuous improvement

At a meaningful cycle closure, collaborators should evaluate transferable lessons without waiting for a separate reminder. Update AICP for collaboration practices, UGDS for applicable product-quality practices, and individual project records for local decisions. Revise only where evidence and impact warrant it; consult AICP §9 for change-control boundaries.

## Commitment Cycle

**Explore → Offer → Execute → Confirm & Close**, with an explicit owner-approved commitment gate between Offer and Execute. Codex contributes feasibility assessments, alternatives and evidence before uncertain implementation; the owner confirms or redirects. See [AICP §6.1](AI-COLLABORATION-PROTOCOL.md). Adoption is versioned and not retroactive.

## Durable development by default

Codex should safely push meaningful intermediate and final checkpoints to a working branch and provide permanent GitHub links before reporting completion. This is preservation, not acceptance or deployment permission. The first Codex brief must both require reading adopted AICP and restate the checkpoint rule. See [AICP §6.2](AI-COLLABORATION-PROTOCOL.md).

## Workspace recovery

AICP §6.3 adds proportionate recovery-ready Git checkpoints, concise handoff pointers and an evidence-first recovery mode when cloud workspaces disappear. A handoff is not implementation authorization. Existing project standards pins do not change automatically.

## Working model

Human creative director owns design and approval; advisory AI challenges and clarifies; Codex evaluates feasibility, implements and reports; the **individual project repository** stores durable approved decisions and evidence. AI memory aids navigation, but is not the authoritative record.

The standards repository holds reusable process and quality rules, **not** confidential personal conversations or project-specific specifications. AICP does not silently modify UGDS 1.0.0.
