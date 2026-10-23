# Codex Implementation Brief — [Game Title]

**Project repository:** [owner/repo]  
**GDD:** [path + pinned version/commit]  
**Universal standard:** [UGDS vX.Y.Z + immutable tag/commit SHA]  
**Assignment:** [POC / full build / revision / release]  
**Authorized branch / deployment target:** [details]

## Governing instructions

Read the pinned UGDS and GDD **before implementation**. Treat both as binding. Do not paraphrase or rewrite the universal standard for this project. If a requirement conflicts, record it and request a decision; do not silently drop a requirement. Project-specific instructions may strengthen UGDS. Only the creative director can approve a scoped exception to a mandatory rule.

## Objective and boundaries
- Deliver:
- Explicitly out of scope:
- Fixed game-design decisions:
- Engineering choices delegated to Codex:
- Known dependencies and risks:

## Required workflow

1. **Inspect and plan.** Confirm the governing versions, repository state, implementation strategy, and potential conflicts.
2. **Validate the core mechanic.** Build a playable functional POC with representative game-state transitions and testable rules. Do not claim the POC's visuals are finished.
3. **Visual production gate.** For visually ambitious games, produce an actual in-engine representative scene at desktop and mobile sizes, including the most difficult interactive objects and meaningful effects. Present the art pipeline, limitations, and screenshots for creative-director approval **before** scaling production. Concept images are references only, never gameplay background substitutes or the visual-quality ceiling.
4. **Build the complete game.** Implement all approved content, English/zh-TW live switching, desktop/touch input, responsive layouts, progress/preferences as applicable, and coherent original artwork.
5. **Verify independently.** Run unit tests, scenario/balance checks when relevant, production build, browser E2E tests with real interactions, both-language playthroughs, layout/accessibility checks, and visual inspection.
6. **Release only when authorized.** Distinguish committing, CI, deploying, and verifying the live URL. Do not infer one from another.
7. **Report evidence and gaps.** Include commit SHA, test counts, actual screenshot paths, live URL only if verified, unresolved risks, and tests not performed.

## Mandatory visual instruction

**Do not use concept images directly as finished levels or gameplay backgrounds.** Do not present generic placeholders or functional-prototype art as production-quality completion. The final in-game composition, asset coherence, perspective, animation, and interaction clarity require independent review. If the chosen pipeline cannot meet the visual direction, escalate alternatives and tradeoffs rather than silently downgrading.

## Escalate before proceeding if
- The art pipeline cannot meet the approved visual direction.
- A material mechanic, difficulty, content, or accessibility requirement must change.
- A mandatory UGDS item appears infeasible.
- The solution requires new paid services, external dependencies with significant risk, accounts, telemetry, or third-party licensed assets.
- The available evidence cannot support a claimed acceptance or deployment result.

Minor engineering details are delegated; no need to ask for approval at every implementation step.

## Acceptance and evidence table

| Area | UGDS IDs | Evidence to provide | Status |
| --- | --- | --- | --- |
| Playable loop / mechanics | P01, P04, P05 | Rules tests + real playthrough | Not Verified |
| Input and layouts | P02, P03 | Desktop/mobile screenshots and interactions | Not Verified |
| Localization | L01, L02 | EN/zh-TW complete gameplay and switching | Not Verified |
| Accessibility | A01, A02 if applicable | Keyboard/touch + audit and limitations | Not Verified |
| Visual quality | V01–V06 | In-engine POC approval, production screenshots, visual review | Not Verified |
| Storage / performance / safety | S01–S04 as applicable | Recovery and performance evidence | Not Verified |
| QA / deployment | Q01–Q06 | Test results, CI, live verification if in scope | Not Verified |
| Collaboration / changes | C01–C03 | Decisions, approvals, exceptions | Not Verified |

Statuses: Pass / Fail / Not Applicable (reason) / Not Verified. Do not mark unperformed checks as passed.

## Final delivery report
- Built:
- Commit / artifact:
- Tests run and results:
- Visual quality review and approval status:
- Live deployment and verification status:
- Known limitations:
- Physical-device / independent-player testing status:
- Follow-up decisions requiring creative-director input:
