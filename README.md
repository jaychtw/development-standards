# Game Development Standards

Central, versioned guidance for AI-assisted games and application projects.

## Governing documents

- [UGDS v1.0.0](UGDS.md) — adopted **game development quality** baseline. Pin the precise UGDS tag or commit in each adopting project; existing projects are not retroactively certified.
- [AI Collaboration & Continuity Protocol (AICP) v1.1.0](AI-COLLABORATION-PROTOCOL.md) — shared AI/human collaboration, memory recovery, decisions, evidence, handoffs and approval boundaries. Applies to games and apps that adopt it.

## Templates

- [GDD](templates/GDD-TEMPLATE.md) — project gameplay/experience and rules.
- [Codex brief](templates/CODEX-BRIEF.md) — bounded implementation assignment.
- [Project state](templates/PROJECT_STATE.md) — lightweight current-state index in each project's repo.
- [Conversation starter](templates/CONVERSATION-STARTER.md) — reusable opening message for a new ChatGPT Game Development conversation.

## Continuous improvement

At a meaningful cycle closure, collaborators should evaluate transferable lessons without waiting for a separate reminder. Update AICP for collaboration practices, UGDS for applicable product-quality practices, and individual project records for local decisions. Revise only where evidence and impact warrant it; consult AICP §9 for change-control boundaries.

## Working model

Human creative director owns design and approval; advisory AI challenges and clarifies; Codex implements and reports; the **individual project repository** stores durable approved decisions and evidence. AI memory aids navigation, but is not the authoritative record.

The standards repository holds reusable process and quality rules, **not** confidential personal conversations or project-specific specifications. AICP does not silently modify UGDS 1.0.0.
