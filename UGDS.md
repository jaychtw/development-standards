# Universal Game Development Standard (UGDS)

**Version:** 2.0.0
**Status:** Adopted risk-proportionate quality baseline for games explicitly adopting v2
**Owner:** Project creative director
**Date:** 2026-11-07

## 1. Intent and precedence

Ship the **specific experience the owner froze**, not a technically polished substitute. The FINAL project GDD defines game rules, presentation, requirements and authorized release. AICP v2 defines the single-gate collaboration model. This UGDS defines **outcome-oriented minimum quality**. Law, safety, platform and privacy obligations take precedence. Pin adopted versions to immutable commits/tags. Versions do not retroactively change existing project requirements.

**MUST** means mandatory unless an explicit owner-approved scoped exception; **WHEN APPLICABLE** applies only to relevant mechanics. No mandatory intermediate owner sign-offs, fixed test counts or boilerplate compliance matrices. Use evidence to detect real defects.

A project must be designated **Release** or **Experiment** at Design Freeze. Default is Release. Experiment may omit explicitly listed release features and publication, but may not be presented as a complete public game. Do not silently downgrade Release to Experiment.

## 2. Game and interaction

- **P01 | Complete loop (MUST):** Start, comprehend controls/goals, act, receive truthful feedback, complete/fail, and replay or recover as the GDD specifies. Test at least one meaningful happy path and one relevant failure/retry path.
- **P02 | Target input (MUST):** Working and discoverable primary controls on all *declared* platforms; if both desktop and mobile are selected, exercise keyboard/mouse and touch-emulated interaction. No hidden hover-only essential action.
- **P03 | Responsive usability (MUST):** Test representative narrow and wide sizes for the declared platform(s); add tablet/orientation/edge sizes where layout risks justify them. No mandatory four-viewport ritual. No obstructed essential controls, illegible playfield or accidental clipping.
- **P04 | Rules integrity (MUST):** Physics, collision, paths, scores, progression, timing and visible indicators agree with the approved GDD and real engine. Core consequential rules have automated tests where feasible. Exercise edge conditions in proportion to risk.
- **P05 | Recoverability (MUST):** Retry/restart and destructive-action handling do not silently corrupt earned progress or leave irrecoverable states.

## 3. Language, accessibility and usability

- **L01 | Language scope (MUST):** The GDD must explicitly select languages at freeze. **English + Traditional Chinese is the recommended default** for this portfolio, not a silent extra requirement for a deliberately single-language experimental game. Localize applicable instructions, HUD, errors, outcomes and accessibility labels from centralized resources. If bilingual, support switching without losing state and test representative complete flows in both languages.
- **A01 | Accessible essentials (MUST):** Legible text, sufficient contrast, visible keyboard focus where keyboard is supported, meaningful labels, appropriate touch targets and no color-only essential signaling. Perform at least one targeted accessibility inspection/audit for the intended interface; inspect critical findings rather than counting scans.
- **A02 | Motion and sound (WHEN APPLICABLE):** Honor reduced-motion preference for nonessential animation, provide practical mute/volume controls when sound exists, and avoid audio-only essential cues.

## 4. Visual and content quality

- **V01 | Frozen art direction (MUST):** Final composition, object readability, styling, perspective, sprites/effects and animation must meet the GDD's **observable** visual requirements. Original or appropriately licensed assets only. An illustration may serve as a final scene if intentionally specified as such; concept art must not accidentally become a substitute for a game-ready environment.
- **V02 | Production-quality evaluation (MUST):** Inspect representative **actual running** desktop/mobile screens for applicable targets and meaningful states. Compare to GDD reference images, examples, acceptable stylistic variation and measurable constraints; keep genuine visual evidence. Functional tests alone do not establish visual quality.
- **V03 | Internal POC, no intermediate human gate:** Codex may build visual or mechanical prototypes privately to validate uncertain production work. **The owner does not have to approve a POC before full implementation.** If truly unresolvable art feasibility would force a change to frozen intent, use AICP exception-only escalation.
- **V04 | No disguised downgrade (MUST):** Never label generic placeholders, missing animations, broken integration, or silently reduced scope as finished. A consciously chosen minimalist style is legitimate when the final GDD specifies it.

## 5. Performance, data and safety

- **S01 | Storage (WHEN APPLICABLE):** Persist required progress and settings; handle invalid/blocked storage safely. Do not add accounts, telemetry or external data transfer without consent.
- **S02 | Runtime (MUST):** Responsive input and adequate performance on declared ordinary target devices; document significant known limitations. Prefer cheap, reproducible, locally bundled approaches when feasible.
- **S03 | Safety and licensing (MUST):** Follow age, content, privacy/security and intellectual-property constraints; do not imply fictional systems demonstrate real-world safety or capability.

## 6. QA and release integrity

- **Q01 | Proportionate evidence (MUST):** At minimum, record (a) production build result; (b) core rule checks where applicable; (c) one real browser/player success and failure/retry exercise; (d) primary input, language and layout checks for declared targets; (e) targeted accessibility findings; (f) representative visual evidence and inspection; (g) known limitations. Expand only for complexity, risk or explicit GDD requirements. **No mandated test-number threshold.**
- **Q02 | Honest status (MUST):** Mark each applicable acceptance outcome Pass / Fail / Not Verified / N/A with reason. Automated audits are not equivalent to human aesthetic review. Physical-device and first-time-player evaluations may remain labeled Not Verified unless the GDD made them release-critical. Never invent approvals, screenshots or independent verification.
- **Q03 | Fix before release (MUST):** All frozen release-critical criteria must pass or have an explicit owner-approved exception. Repair and rerun relevant tests; do not ship failed essential mechanics, significant accessibility barriers or misrepresented art completion.
- **Q04 | Publish only with advance or fresh authorization (MUST):** Source commit, PR/merge, CI, deployment and actual live interaction are different states. A frozen GDD may preauthorize the exact deployment, visibility and destination; it does not bypass branch protection or payment/account controls. Verify live URL + representative action before claiming publicly released. Do not deploy unapproved services or publish unrelated portfolio changes.

## 7. Agency, escalation and definition of done

Codex decides internal architecture, asset pipeline, test selection, bug fixes, branch checkpoints and internal prototype sequence. The owner decides frozen creative outcome, acceptable fallback, budgets and exposure **during Design & Decide**. After freeze, refer to AICP v2 exception-only escalation. A failed constraint is not permission to weaken the product.

**Complete** means the full frozen Release scope is implemented, mandatory applicable quality criteria are met, evidence is truthful, the final source is durably pushed and any **preauthorized** publication is verified. No second ordinary human acceptance gate. If protected branch merge or hosting is blocked, report a verified deployable handoff and mark publication blocked—not complete.

**This revision supersedes UGDS v1's obligatory intermediate visual approval, four specified viewport widths, unconditional bilingual requirement, and extended blanket testing ceremony for projects adopting v2.** Existing pinned v1 projects are unaffected.
