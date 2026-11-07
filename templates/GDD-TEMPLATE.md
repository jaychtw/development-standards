# [Project Title] — FINAL Game / App Design & Delivery Contract

**Status:** FINAL — owner-approved at Design Freeze (do not create a Draft GDD)
**Freeze date and authorization evidence:** [date + conversation/approval reference]
**Project repository and source visibility:** [owner/repo, public/private]
**AICP / UGDS adoption:** [exact version + immutable commit/tag; UGDS only for games or explicitly adopted app provisions]
**Release mode:** Release / Experiment (default Release)

> Work through AICP v2's design-completeness questions *in conversation*, before creating this file. Empty placeholders are not decisions. Omit truly irrelevant sections, but do not leave consequential choices unresolved or invite post-build design negotiation. The FINAL GDD is the sole owner-approved product/design authority; Codex decides only bounded implementation details.

## 1. Product identity
- Pitch and what makes it distinctive:
- Intended audience, emotional or practical experience and session/use pattern:
- Owner's exact relevant examples and creative references (with source links):
- Non-goals and explicitly excluded features:

## 2. Complete interaction specification
- Onboarding, start, main user journey/core loop, success/completion, failure/retry, exit/restart:
- All user actions, controls and feedback (desktop/touch where required):
- Entities, states, rules, timing, quantities, difficulty, scoring/progression and content inventory:
- Edge cases, invalid actions, persistence, recovery and expected fallback behavior:
- For apps: workflows, data sources, errors, permissions and offline/network handling:
- Critical screens, navigation, copy and interaction outcomes:

## 3. Look, feel and content
- Visual direction, references, composition/camera/perspective, layout and required assets:
- Explicit observable finish criteria (what would count as visually wrong):
- Animation, effects, audio, sound control and reduced-motion behavior:
- Content inventory and accepted source/provenance/license constraints:

## 4. Platforms, quality and architecture boundaries
- Target devices, viewport/orientation coverage and input modalities:
- Languages (portfolio default EN + zh-TW; specify whether live switching applies):
- Accessibility, privacy/security, performance, storage and offline expectations:
- Approved technology/budget/dependency constraints:
- Engineering methods **delegated to Codex**:
- Explicit fallback hierarchy for foreseeable constraints (equivalent substitutions only):

## 5. Acceptance contract (decided BEFORE build)
- Must-pass end-to-end success and failure/retry scenarios:
- Core logic test scenarios and challenging edge cases:
- Actual layout, language, accessibility and visual checks:
- Release-critical criteria, allowable limitations, and tests not required:
- Definition of finished release, with no implied follow-on phase:

## 6. Release authorization — explicit, not inferred
| Action | Authorized at freeze? | Exact target, constraints and required checks |
| --- | --- | --- |
| Full implementation and safe working-branch pushes | Yes / No | [repo, branch policy] |
| PR / merge to release branch | Yes / No | [protected-branch requirements; no bypass] |
| Public/private deployment and hosting | Yes / No | [exact hosting, URL/path, visibility, credentials policy] |
| Possibility catalog update / independent publish | Yes / No | [portal repo, Games/Apps, approved artwork or fallback, portal policy] |
| External services / data sharing / spend | Yes / No | [explicit services, scope, $0 ceiling by default] |

Do not interpret blanks or "TBD" as authorization. If a step is not authorized, Codex must not execute that step, but should complete authorized work and report the precise final handoff.

## 7. Hard stops and decisions locked at freeze
- Material design changes Codex **cannot** decide:
- Preapproved alternatives/fallbacks Codex **can** decide:
- Genuine escalation triggers: cost, safety, privacy, access, licenses, unresolvable creative change, unapproved public destination:
- Final owner Design Freeze approval reference:

**Handoff:** At the exact time this FINAL GDD is produced, ChatGPT also produces the companion ready-to-run Codex brief from templates/CODEX-BRIEF.md. Do not require the owner to ask for it or return for normal design clarification.
