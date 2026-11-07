# Game Development Standards

Central, versioned guidance for **design-first, one-shot AI-assisted games and apps**.

## Proposed v2: one creative decision gate, autonomous delivery

**Design & Decide → Design Freeze → Build, Verify & Publish.** The owner and ChatGPT resolve foreseeable design choices *before* producing a FINAL GDD. ChatGPT automatically includes the companion Codex execution prompt. Codex then implements, self-corrects, verifies and (when the exact destinations and permissions were preauthorized at freeze) publishes without recurring owner review cycles.

- [AICP v2](AI-COLLABORATION-PROTOCOL.md) — one planned approval gate, decision completeness, bounded autonomy, escalation only for real exceptions, safe release and continuity.
- [UGDS v2](UGDS.md) — release-quality outcomes, proportionate tests, internally verified visual production, no compulsory intermediate owner visual approval.
- [Final GDD template](templates/GDD-TEMPLATE.md) — no mandatory draft; freezes product and release authorization.
- [Automatic companion Codex brief](templates/CODEX-BRIEF.md) — one-shot end-to-end execution.
- [Conversation starter](templates/CONVERSATION-STARTER.md) — use at the beginning of a design-only conversation.
- [Minimal project state](templates/PROJECT_STATE.md) — optional recovery and verified outcome pointer.

**Important:** This branch proposes **AICP/UGDS 2.0.0**. It is not an adopted baseline merely by existing in a PR. Prior adopted AICP v1.5.0 and UGDS v1.0.0, and the projects pinned to them, do not change automatically. After merge, pin the exact resulting commit/tag for any new adoption and explicitly authorize migration of old projects.

## How the boundary works

Human decisions happen before freeze: vision, mechanics, aesthetic bar, platforms, scope, fallbacks, budget, source repo and public release destinations. AI decisions happen afterwards: architecture, internal prototypes, assets and integration, test coverage, rework, Git recovery and authorized publishing. Codex must stop only for material, unresolved changes or safety/access/cost constraints; it cannot bypass hosting protections or fabricate verification.

A project release and a Possibility (https://github.com/jaychtw/jaychtw.github.io) catalog entry are distinct operations, but **both can be authorized upfront** during the same freeze.

## Optional agent resources

- [Three.js Game Skills selection guide](references/THREEJS-GAME-SKILLS.md) — optional technical reference. Evaluate fit, license, security, maintainability and $0 constraints; no automatic installation.

## Governance

Use reviewable versioned changes for standards and preserve prior historical revisions. No silent replacement of old project pins. Prefer removing obsolete obligations to adding exceptions. Protect creative momentum **and** truthful safety/QA evidence; neither requires the owner to operate the agent's internal workflow.
