# [Game Title] — Game Design Document

**GDD version:** 0.1.0  
**Status:** Draft  
**Universal standard:** UGDS v1.0.0, pinned to tag/commit: [SHA or release URL]  
**Creative director:** [Owner]  
**Date:** [YYYY-MM-DD]

> This GDD describes the game-specific experience. Do not duplicate UGDS. Reference its requirement IDs when adding stricter rules or requesting an exception. Keep this template proportionate: brief projects may combine or omit non-applicable sections; never omit material game rules, owner decisions or applicable mandatory requirements.

## Governing standards and requirements

This project adopts the **Universal Game Development Standard (UGDS) [version]**, maintained at https://github.com/jaychtw/game-development-standards and pinned to **[immutable tag and commit SHA]**. The GDD defines this game's creative direction, mechanics, content, and project-specific requirements; UGDS governs reusable development, localization, accessibility, visual-production, quality-assurance, and delivery requirements.

**For matters not specified or fully detailed in this GDD, the applicable UGDS requirements shall govern.** Applicable laws, regulations, platform policies, and safety requirements also apply and take precedence where required. The GDD may add more specific or stricter requirements, but cannot silently waive mandatory UGDS requirements.

If a GDD requirement appears to conflict with UGDS, **pause implementation of the affected matter**, document the conflict, and obtain the creative director's decision and any expressly approved exception. Neither omission, ambiguity, nor inability to access UGDS constitutes permission to disregard it. **Codex must verify access to and read the pinned UGDS before any implementation begins.**

## 1. One-sentence pitch
[What the player does, and why it is interesting.]

## 2. Audience and intended experience
- Target players / age:
- Primary platform and orientation:
- Emotional tone and session length:
- What the game is **not**:

## 3. Core loop and controls
- Start / tutorial:
- Player decisions:
- State changes and feedback:
- Win / lose / retry:
- Desktop input:
- Touch input:
- Accessibility adaptations:

## 4. Rules and game state
- Board/world representation:
- Entities and their attributes:
- Valid actions and turn/timing order:
- Constraints, scoring, and progression:
- Determinism/randomness and visibility:
- Edge cases and failure recovery:

## 5. Content and difficulty
- Levels / missions / chapters:
- Difficulty curve:
- Hint/assistance approach:
- Replay or practice:
- Balance / solvability acceptance:

## 6. Visual direction and production
- Style and visual references (reference only, not production assets):
- Camera/perspective and composition:
- Required assets, animation, and effects:
- Gameplay readability and touch-target requirements:
- Representative **in-engine** visual POC scene:
- Production pipeline options and risks:
- Visual acceptance criteria and approval checkpoint:
- Originality / licensing considerations:

**UGDS-V01–V06 apply. Prototype completion is not final visual acceptance.**

## 7. Sound and motion
- Sound and mute behavior (if applicable):
- Animation and reduced-motion behavior:

## 8. Localization
- Project terminology in English and zh-TW:
- Text expansion or font concerns:
- Dynamic and contextual messages:

**UGDS-L01–L02 apply.**

## 9. Progress and technical boundaries
- Save/resume behavior:
- Offline/network expectations:
- Device/performance targets:
- Technology restrictions, if any:
- Explicitly excluded features:

## 10. QA and acceptance
- Core engine tests:
- End-to-end browser scenarios:
- Full campaign/playthrough coverage:
- Layout and accessibility checks:
- Visual review and screenshot checklist:
- Build, CI, and live deployment verification:
- Outstanding human/physical-device testing:

## 11. Decisions and risks
| Decision or risk | Owner | Status | Resolution / acceptance |
| --- | --- | --- | --- |
| [Example] | [Owner] | Open | [Next step] |

## 12. UGDS applicability and exceptions
| Requirement ID | Status (Applies / N/A / Exception requested) | Rationale / approval |
| --- | --- | --- |
| [UGDS-...] | [Status] | [Evidence or reason] |

No mandatory requirement is waived without documented creative-director approval.

## 13. Definition of v1.0
[Smallest complete, polished, verified release. Keep possible future modes out of scope unless approved.]
