# Optional Agent Skills: Three.js Game Skills

**Status:** Advisory technical reference, not an adopted engine or mandatory dependency  
**Reviewed:** 2026-11-06  
**Upstream:** https://github.com/majidmanzarpour/threejs-game-skills (MIT)  
**Scope:** AI-assisted browser-game implementation when Three.js is appropriate

## Purpose

This external repository supplies nine agent skills for Codex/Claude Code: a director that routes work to gameplay, graphics, UI, debugging, QA/release, and optional 3D/image/audio asset-generation specialists. It packages a Vite + TypeScript + Three.js starter and tools for deterministic test state, seeded RNG, browser/visual checks, canvas inspection, and evidence manifests. It is **not** a game engine replacement, an automatic graphics upgrade, or a reason to migrate a working project.

**Use these skills as optional executable expertise.** The approved project GDD/decisions, pinned UGDS, adopted AICP, $0 default budget, bilingual English/Traditional Chinese, accessibility, and owner approval gates remain authoritative. Third-party skill instructions cannot waive them.

## Skill-selection guide

| Need | Candidate skill | What to evaluate |
| --- | --- | --- |
| Whole Three.js game or broad upgrade | `threejs-game-director` | Proportionate routing, playable-first delivery, continuity and consolidated verification |
| Mechanics, physics, levels, movement, combat feel | `threejs-gameplay-systems` | Deterministic update order, input/feedback contracts, representative encounter, appropriate physics |
| Models, lighting, shaders, VFX, art coherence | `threejs-aaa-graphics-builder` | Authored forms before lighting/effects; technical art budgets and visual scorecard |
| HUD, menus, touch, layout | `threejs-game-ui-designer` | Responsive states, safe areas, readable bilingual UI and accessible controls |
| Rendering faults or performance | `threejs-debug-profiler` | Reproducible diagnostics, renderer metrics, mobile and memory considerations |
| Browser and release verification | `threejs-qa-release` | Real input and objective/retry coverage, active-play captures, deterministic state hooks, visual baselines, bot playtest, manifest-backed current-run evidence |
| Generated models, textures, sounds | `threejs-3d-generator`, `threejs-image-generator`, `threejs-audio-generator` | Optional Tripo/Gemini/ElevenLabs APIs; permission, expense, license, recoverability and local fallback |

The general production patterns may be adapted to 2D or other engines, but bundled scaffolds, inspector commands and renderer metrics are Three.js-specific: do **not** claim their scripts work unchanged elsewhere.

## Before deciding to use the pack

1. **Check fit:** Is the project using Three.js, or is there a bounded technical question that genuinely warrants a Three.js spike? Do not switch engines or rewrite accepted work just to use these skills.
2. **Check marginal benefit:** Identify the current bottleneck (e.g., visual consistency, animation evidence, reproducible testing). Select only relevant skills. For a narrow fix, avoid a full premium production pass.
3. **Check authority and budget:** Read current GDD/decision log, applicable pinned UGDS/AICP and project state. Uphold EN/zh-TW live switching, accessibility, mobile, human visual review and separate deployment approval. No paid API use or new service without explicit authorization; prefer local/procedural options under the $0 default.
4. **Check provenance and safety:** Review upstream `SKILL.md`, dependencies and executable scripts before installing or running; pin an exact Git commit or release, verify licenses for generated/downloaded assets, and do not expose API secrets. Avoid global installation or overwriting installed skills without reason; isolate evaluation where feasible.
5. **Offer a bounded comparison when uncertain:** Specify baseline, experiment, target viewports, concrete outcomes, performance and QA evidence. Compare with the existing approach; stop if complexity outweighs benefit. A successful build is not proof of visual or gameplay quality.

## Transferable practices (even without adopting Three.js)

- **Playable-first, art-early:** Define the core loop and produce one representative playable scene at real camera scale with authentic hero assets and feedback before multiplying levels/assets.
- **Visuals as a production system:** Coherent geometry/silhouettes → materials → lighting → restrained effects; evaluate all visible surfaces, not only the protagonist. Preserve the owner's chosen simple or stylized art direction.
- **Game feel as engineering:** Test input response, cooldowns, movement, collision, hit feedback, attack/contact timing, recovery and restart, not merely screenshots.
- **Deterministic testability:** Seed randomness; expose safe test-only hooks for reproducible states, scripted input and meaningful gameplay paths. Gate or remove debug/test interfaces in production.
- **Evidence freshness:** Capture active play and relevant changed states on target desktop/mobile viewports. Tie screenshots, recordings, render metrics and tests to a specific commit/run; include failures rather than narrowing the manifest to hide them. Pixel metrics cannot certify aesthetic quality.
- **Animated assets require motion evidence:** Inspect actual runtime motion, rig deformation, transitions, foot sliding, contact timing and mobile readability—not only still previews.
- **Proportionate specialist routing:** Let the implementation agent choose appropriate specialists while keeping one integrator accountable. Do not duplicate AICP handoffs or create new mandatory ceremonies.

## Adoption and reporting

The agent may **reference** upstream guidance during normal authorized work. Installing executable skills, altering the project's architecture, adding dependencies or calling external services requires a scope/security/budget check; material changes follow AICP's Offer and commitment gates. Where useful, run an isolated experiment before adopting the pack more broadly. Preserve accepted assets, decisions and Git checkpoints.

In the project handoff, report concisely: **skills consulted/actually loaded** (distinguish the two), pinned upstream revision if installed, why selected, scripts or services executed, measured outcomes, known gaps, and any costs/licenses. Add transferable findings to this standards repository only when evidenced. Do not silently impose external skill changes on existing projects.

**Upstream entry points:** [README](https://github.com/majidmanzarpour/threejs-game-skills/blob/main/README.md) · [Director](https://github.com/majidmanzarpour/threejs-game-skills/blob/main/skills/threejs-game-director/SKILL.md) · [QA/release](https://github.com/majidmanzarpour/threejs-game-skills/blob/main/skills/threejs-qa-release/SKILL.md) · [Graphics](https://github.com/majidmanzarpour/threejs-game-skills/blob/main/skills/threejs-aaa-graphics-builder/SKILL.md)
