# Codex Implementation Brief — [Game Title]

**Project repository:** [owner/repo]  
**GDD:** [path + pinned version/commit]  
**Universal standard:** [UGDS vX.Y.Z + immutable tag/commit SHA]  
**Assignment:** [POC / full build / revision / release]  
**Authorized branch / deployment target:** [details]

## Governing instructions

Read the pinned UGDS and GDD **before implementation**. Treat both as binding. Do not paraphrase or rewrite the universal standard for this project. If a requirement conflicts, record it and request a decision; do not silently drop a requirement. Project-specific instructions may strengthen UGDS. Only the creative director can approve a scoped exception to a mandatory rule.

## Mandatory UGDS preflight — blocking prerequisite

**No verified UGDS, no implementation.** This applies to all assignments, including prototypes. Do not begin coding, asset production, or game implementation until the following checks succeed:

1. Access the standards repository at https://github.com/jaychtw/game-development-standards (private; request authorization if needed).
2. Retrieve **the exact pinned UGDS version and commit SHA** listed above. Never substitute the current `main` branch for a pinned release.
3. Verify the retrieved document belongs to the pinned commit, and read **UGDS.md in full**, together with the project GDD and this brief.
4. Identify material conflicts, missing requirements, and any proposed exceptions. Resolve blocking issues with the creative director before implementing affected work.
5. Record preflight evidence in the delivery report: source URL, tag, resolved commit SHA, confirmation of full read, and conflict/exception status.

**Access or verification failure:** Stop before implementation; report the exact problem, request authorization or an approved alternate means of obtaining the pinned document, then retry. Do not reconstruct UGDS from memory, earlier games, summaries, or assumptions. Do not use the GDD as a substitute. Permission to access the project repository does not necessarily grant access to the separate private standards repository.

### Trackmaster pilot onboarding note (include only in its initial handoff)

Trackmaster is the first game under a new two-document requirements workflow. Earlier games relied principally on their individual GDDs. For Trackmaster, both UGDS v1.0.0 (tag `v1.0.0`, commit `d5c6696efdd6efc028118600466db44aecae0c9b`) and its project GDD are binding. Explicitly acknowledge successful preflight before continuing. **Trackmaster must meet its own game-quality goals; it is not merely a process test.**

## Commitment Cycle preflight (proportionate)

- **Explore:** What owner-approved intent or candidate GDD is being evaluated? Which assumptions remain unproven?
- **Offer:** What can Codex demonstrably deliver with the available environment, budget and tools? Identify material uncertainties, alternatives/counteroffers and whether a bounded technical spike is warranted.
- **Commitment gate:** Record owner-approved scope, exclusions, constraints, evidence, acceptance criteria, stopping conditions and release permissions. An assessment-only assignment does not authorize implementation.
- **Execute:** Implement only the agreed commitment and report deviations or a revised offer when assumptions fail.
- **Confirm & Close:** Present reproducible technical and visual evidence for owner review; record accepted, conditional, rejected or reopened outcome. Separate milestone acceptance from final quality and deployment authority.

## Objective and boundaries
- Deliver:
- Explicitly out of scope:
- Fixed game-design decisions:
- Engineering choices delegated to Codex:
- Known dependencies and risks:

## Git checkpoint delivery

Read adopted AICP §6.2. Use a dedicated working branch, check CI/deployment and secret risks, and safely push intermediate and final checkpoints before reporting completion. Provide verified GitHub links. Do not force-push, merge or deploy without approval. If unsafe, report the blocker and independent backup status.

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

## Preflight verification record
- UGDS repository and document URL:
- Pinned tag / resolved commit SHA:
- Full UGDS read: Confirmed / Blocked (explain)
- GDD and brief read: Confirmed / Blocked (explain)
- Conflicts / approved exceptions:
- Preflight outcome: Passed / Blocked
- Implementation started only after preflight: Yes / No (explain)

## Offer and closure record
- Feasibility uncertainties and evidence / spike outcome:
- Codex offer or counteroffer and tradeoffs:
- Owner commitment authorization and scope:
- Owner confirmation status (accepted / conditional / rejected / pending):
- Accepted baseline and independent follow-up commitments:
- Reopened stage and rationale, if applicable:
- Separate merge / release / deployment authorization:

## Final delivery report
- Built:
- Commit / artifact:
- Tests run and results:
- Visual quality review and approval status:
- Live deployment and verification status:
- Known limitations:
- Physical-device / independent-player testing status:
- Follow-up decisions requiring creative-director input:
