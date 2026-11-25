# Development Standards

These standards guide AI-assisted work on games and apps. The owner can explore an idea, authorize a build, inspect the result and request revisions in one conversation. The same assistant carries the work through implementation and verification. This workflow can be used across model generations.

## Starting from the owner's request

| What the owner brings | How to proceed |
| --- | --- |
| “I have an idea. What do you think?” | Explore the experience and tradeoffs. Wait for a build instruction. |
| “Use this HTML as module 2 and keep module 1 playable.” | Inspect the supplied file and existing routes, integrate the module, then exercise both entry points. |
| “The game opens with a blank canvas.” | Reproduce it at the reported route, repair the cause and verify a visible, interactive scene. |
| “Freeze this design” or “hand this to another agent.” | Record the agreed design or prepare the requested transfer. Carry forward the exact scope and permissions. |

## Which document to use

- [AI Collaboration & Continuity Protocol (AICP 3.0.0)](AI-COLLABORATION-PROTOCOL.md) defines who decides, how to iterate, when to ask and how to recover and release.
- [Universal Game Development Standard (UGDS 2.1.0)](UGDS.md) defines game quality and verification. Apps can adopt relevant provisions.
- [Conversation starter](templates/CONVERSATION-STARTER.md) gives an optional opening for new and existing projects.
- [Design contract](templates/GDD-TEMPLATE.md) records a substantial agreed design when useful or requested.
- [Handoff brief](templates/CODEX-BRIEF.md) transfers work when the person, session or environment changes.
- [Project state](templates/PROJECT_STATE.md) indexes the last checkpoint when a project needs a recovery record.
- [Capability registry](references/CAPABILITY-REGISTRY.md), [Diorama](references/DIORAMA-THREEJS.md), [Three.js skills](references/THREEJS-GAME-SKILLS.md) and [runtime identity](references/RUNTIME-IDENTITY-AND-CACHE.md) are optional engineering references.

## Adoption

Pin the standards commit in the project when adopting this edition (2026-11-25). Existing pins continue to govern until the owner chooses to migrate. Preserve project-specific decisions and release permissions during migration. See the [changelog](CHANGELOG.md).
