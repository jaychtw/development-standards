# Capability Registry — optional external resources

**Status:** Curated advisory reference; initially reviewed 2026-11-06. Evidence and upstream conditions may age.

The purpose of this small index is to help collaborating agents **reuse proven methods instead of independently rediscovering them**. It is neither an approved-dependency list nor a mandatory research task. Project design and source truth take precedence. Search beyond these entries when appropriate.

## Find a starting point by problem

| Need | Resource | Practical uses | Evidence level |
| --- | --- | --- | --- |
| Three.js game architecture, gameplay, 3D art/graphics, browser QA or performance diagnostics | [Three.js Game Skills](https://github.com/majidmanzarpour/threejs-game-skills) | Specialist agent instructions and reproducible production/testing patterns; see [local assessment](THREEJS-GAME-SKILLS.md) | Reviewed upstream (2026-11-06); not automatically proven for a particular project |
| Stylized 3D dioramas, procedural scene construction, character/vehicle motion, water presentation and frame-level visual QA | [Diorama](https://github.com/sloemo01/diorama) | Three.js scene playbook, copy-in modules and deterministic frame/contact checks; see [local assessment](DIORAMA-THREEJS.md) | Source-reviewed (2026-11-13); no runtime validation in portfolio games |
| Pixel-art combat effects, explosions, impacts, spells, spritesheet export and effect timings | [PixelFX](https://github.com/patch-gg/pixelfx) and [gallery](https://patch-gg.github.io/pixelfx/) | Select a reference effect, study/adapt code or export appropriate transparent frames | Reviewed upstream (2026-11-06); actual project integration must be verified |

**Three.js Game Skills:** primarily aligned to Three.js/Vite/TypeScript. Consider only relevant skills, not a full suite by default; optional external model/asset services can cost money. Review upstream source, exact revision, license and any executable scripts before adopting. Useful ideas may also be applied without installing a skill.

**Diorama:** a specialized Three.js procedural scene and visual-verification toolkit, not a general game engine. Treat its render-style and model-sourcing prompts as optional project-specific guidance rather than extra gates; follow the owner's already-approved art direction and the agreed project scope. Its MIT code license does not automatically license external models or recognizable example characters. Inspect and pin chosen modules before reuse.

**PixelFX:** a gallery of code-defined pixel effects. When the owner points to a specific example, treat it as a **creative reference**, not an instruction to clone unrelated copyrighted assets or change the engine. Possible implementation routes include adapting effect source, using the compatible renderer, or producing a source-backed sprite sheet. Confirm existing licenses/NOTICE and third-party exceptions from the actual revision before use; visually validate style, scale and animation in the destination game.

## Select proportionately

1. Identify the actual project problem and current engine/tool constraints. Do not start an external research campaign for a routine local fix.
2. Distinguish **reference only** (learning from a resource), **bounded adaptation** (reusing a component or asset) and **executing/installing a dependency/skill**. Favor the lightest method that serves the required result.
3. Before running external code, inspect untrusted instructions/scripts, provenance, license, version, security, privacy, budget, maintainability and integration costs. Do not expose credentials, silently add paid calls, or overwrite a working project just because a capability exists.
4. Validate in the *actual* target experience using proportional real-input, visual, accessibility, language, performance and regression checks **as applicable to the agreed project requirements**. No new owner-facing POC approval gate.
5. Record only reusable evidence: problem, exact resource revision, what was actually used, project commit, observed outcomes, limitations and failure modes. Mark **Proven** only for the specific demonstrated capability, not a whole library.

## Authority and upkeep

An owner-provided visual/interaction reference has priority as creative intent but is **not** automatic permission to install software or change public release scope. An agent-discovered technical resource is advisory until explicitly integrated under the agreed design and authorized tool/budget boundaries. The $0 default, legitimate licensing, confidentiality, access controls, durable source custody and honest evidence remain in force.

Keep the registry small. Update or prune entries after a meaningful new resource, verified experience or discovered change; **do not invent new required forms, experiments, audits or approval stages**. Agents can independently use other credible external resources.

**Useful entry fields if needed:** resource and canonical URL, find-when keywords, provided capability, stack fit, evidence level/source, risk/license/cost constraints, and last verification. No standalone ADR is required for each entry.
