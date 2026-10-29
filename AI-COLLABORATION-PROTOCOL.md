# AI Collaboration & Continuity Protocol (AICP)

**Version:** 1.0.0  
**Status:** Adopted collaboration baseline  
**Applies to:** AI-assisted game and application development adopting this protocol  
**Owner:** Human product owner / creative director  
**Date:** 2026-10-29

## 1. Purpose and boundaries

Preserve durable design intent, decision rationale and accountable delivery across ChatGPT conversations and AI agents. This protocol governs *collaboration and knowledge continuity*, not gameplay acceptance. UGDS governs applicable game quality standards; the product GDD governs project identity and approved functionality. For non-game apps, apply only expressly adopted UGDS provisions.

**Core rule:** Memory enables familiarity; project documentation establishes authority; implementation and evidence establish what exists.

No AI may claim complete historical recall, successful document retrieval, or owner approval without evidence. Never substitute inferred recollections for verified records.

## 2. Roles and decision ownership

- **Human owner:** vision, design direction, constraints, scope, budgets, acceptance, release and exceptions.
- **ChatGPT / advisory AI:** challenge assumptions, surface tradeoffs and blind spots, maintain decision clarity, create actionable briefs and review evidence.
- **Codex / implementation AI:** implement within approved boundaries, test, document and report deviations and limitations.
- **GitHub:** versioned source of truth for project specifications, decisions, implementation and evidence.

AI agents must not reinterpret delivery as approval. Material scope or gameplay changes, visual direction, costs, external services, deployment, security/privacy impacts or standards exceptions require owner approval. Routine implementation details need not interrupt work.

## 3. Authority, conflicts and evidence

Apply law, safety and platform policy first. For product intent, prefer the owner's latest *explicitly approved* decision, as recorded in project GDD/decision records; then pinned applicable standards and approved briefs. For actual behavior and status, inspect code, builds, tests and deployment evidence. A chat recollection is supporting context, not proof.

Where documentation, conversation, implementation or results disagree:
1. State the conflict and cite the affected records.
2. Distinguish **approved intent**, **implemented behavior**, **verified outcome**, and **unresolved questions**.
3. Never silently choose or rewrite a decision; request owner resolution when material.

Pin the UGDS version by tag or commit SHA as UGDS requires. Pin this protocol by version and preferably commit SHA when reproducibility matters. New standard revisions are not retroactively imposed.

## 4. Context reconstruction on conversation startup

For an existing project:
1. Identify the project repository and review its README, `PROJECT_STATE.md` if present, current GDD, decision records, standards pins, key verification reports and relevant changes.
2. Review this protocol, the applicable UGDS and available project templates.
3. Recover relevant ChatGPT Project conversations when accessible; explicitly distinguish confirmed history from partial memories and inference.
4. Summarize verified phase/status, frozen decisions, known risks and next open question briefly; then follow the owner's instruction.
5. If GitHub or past conversations are inaccessible, declare that limitation. Do not invent missing content or needlessly demand a full recap.

For a new project, establish the scope and governing standards without prematurely restricting exploration. A new conversation per development effort is recommended, not mandatory. If a conversation reaches context limits, use a documented handoff.

## 5. Decision preservation

Record *material* decisions in the project's GDD or decision log, noting:
- identifier/date, decision and status (**proposed**, **approved**, **superseded**, **rejected**, **deferred**);
- rationale and significant alternatives considered;
- consequences, constraints and references to supporting evidence;
- owner approval and superseding decision, when applicable.

Do not mistake brainstorming, agent recommendations or generated files for approved choices. Do not reopen settled decisions absent changed evidence, changed circumstances or an explicit request.

Update `PROJECT_STATE.md` at meaningful milestones or after decisions that change project direction. It is an **index and snapshot**, not a second GDD. Avoid copying entire specifications into it. Keep it compact and link to authoritative files. Treat stale or contradictory state as a review issue, not truth.

## 6. Work and quality gates

Distinguish **exploration → proposed design → owner-approved scope → Codex implementation → verified tests → owner acceptance → deployment approval**. Never collapse these gates. Passing automated tests is not proof of visual quality, user experience or public readiness.

Implementation briefs must contain objective, constraints, authoritative sources, in/out of scope, acceptance tests, evidence requirements, escalation thresholds and stopping conditions. Codex may choose low-impact technical approaches; report design-affecting deviations before implementing them.

On completion, review changes and evidence independently where practical. Label tests as reported, independently reproduced, not verified or failed. Release requires separate authorization.

## 7. Handoff, drift and confidentiality

When transitioning conversations, prepare a concise handoff covering project link, source revision, current phase, accepted decisions, rejected/deferred alternatives, reasoning, pending approvals, risks and next action. Link documents rather than replicate them. If not possible, say what was not recovered.

Do not put credentials, personal data, access tokens or sensitive private discussions into repository records. Verify repository visibility and intended audience before adding content. Private repositories are not a substitute for secret management.

Agents must not claim they persist independent memory across sessions. The recoverable record is the documented Git history, not the model's internal recollection.

## 8. Maintenance and amendment

Reusable process lessons belong here, with a version change and changelog entry. Product-specific decisions belong in their individual repositories. Changes to this protocol require owner review; agents should propose improvements without silently modifying the governing baseline.

**Governing maxim:** Standardize continuity without standardizing creativity.
