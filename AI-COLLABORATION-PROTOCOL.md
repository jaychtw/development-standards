# AI Collaboration & Continuity Protocol (AICP)

**Version 3.0.0 · Adopted 2026-11-25 · Games and apps**

## 1. Follow the request

The owner directs the experience, audience, exclusions, budget and exposure. One assistant can discuss the design, edit the repository, test the result and deliver it in the same conversation. Choose tools and reasoning effort to suit the task. The protocol assumes no particular model or interface.

An exploratory question calls for discussion. An instruction to build, fix or revise authorizes work within its stated scope. “Go for it” after a concrete proposal can authorize that proposal. Read it in context. For existing work, inspect the current files, adopted standards, relevant history and repository instructions before relying on memory. Use a supplied specification, asset or implementation as the starting point.

## 2. Decide what matters

For a new experience, establish the main user journey, the choices that give it character and what the owner expects to see or do when it works. Identify consequential unknowns about content, art, inputs, languages, data, accessibility or feasibility. Explore alternatives while the owner is designing. Once the requested change is clear, choose reversible implementation details and proceed. Ask one focused question when the answer would materially change the outcome and existing decisions provide no answer.

A repair can be scoped by the reported behavior and the expected result. A prototype can be scoped by the question it must answer. For a larger build, keep interdependent rules, approved references, fallbacks and acceptance examples together in a project specification. Use a formal Design Freeze when the owner requests it or chooses to adopt a fixed baseline. Record a FINAL design only after agreement. A direct build can proceed from the request or existing specification without creating a GDD or a second prompt.

## 3. Build and iterate

Implement the authorized change through the real entry point. Preserve existing modules, routes, saved data and behavior outside the change. Use internal prototypes to resolve uncertainty. Give the owner a preview when the request calls for a judgment about feel, look or direction. When feedback arrives, apply it to the current build and rerun the affected checks. Record material revisions to an agreed baseline so a later session can tell which decision superseded which.

If an approach fails, repair it, use an agreed fallback or choose an equivalent implementation. Escalate before sacrificing a defining feature, spending beyond the approved ceiling ($0 by default), exposing private data, changing license terms or taking an unauthorized destructive or public action. Explain the blocked choice and its consequences. Continue independent authorized work.

## 4. Preserve sources and continuity

Inspect branch rules and deployment triggers before writing. Use authorized branches and meaningful remote checkpoints for long-running work. Preserve exact accepted asset bytes, editable sources, provenance and reproducible build inputs at authorized locations. Verify that the running product uses the accepted asset. If only a preview is accessible and fidelity depends on the original, identify the missing file.

After an interruption, reconcile the current branch, commit, files, owner decisions and outstanding checks. Rerun checks where the state has changed. An optional [state index](templates/PROJECT_STATE.md) can point to this evidence. Create a [handoff brief](templates/CODEX-BRIEF.md) only for a real transfer or at the owner's request. Include what the recipient needs to resume without asking the owner to relay artifacts or restate decisions. Keep secrets and private conversation text out of public repositories.

## 5. Verify the experience

Use the project's acceptance criteria and applicable [UGDS](UGDS.md). For a repair, reproduce the reported symptom where possible and exercise the corrected path plus nearby behavior at risk. For a release, run the production build where applicable, exercise a meaningful success and failure/recovery path, and check declared languages, input methods, accessibility and layouts. Inspect the running visuals against the agreed references. A loading screen, successful build or HTTP response alone cannot establish that a game plays.

Repair failures and repeat the relevant check. Distinguish passed, failed, unverified and inapplicable checks. Identify any release-critical gap and obtain an explicit scoped exception before releasing with it. Attribute personal visual approval only to someone who actually reviewed the result.

## 6. Publish within the owner's authorization

Track repository writes, merge, project deployment and portal publication independently. Authorization can arrive upfront or later in the same conversation. Carry it forward with the exact destination, visibility and scope. Respect branch protections, hosting controls, licensing, privacy and spend limits. If a push would automatically publish outside the authorization, use a safe branch.

For an authorized project release, verify the deployed route and a representative action. For a catalog request, use the named portal and section, follow its current localization and artwork conventions, and verify the live card opens the intended project. Jolly Chubby Studio is the public studio portal. Possibility is a separate destination. Naming one grants no authority over the other.

Close with the source revision, what works, checks performed, material limitations and each requested publication result. Report a blocked deployment separately from completed implementation.

## 7. Maintain shared standards

A project can preserve a reproducible lesson locally. When the owner delegates portfolio-wide maintenance, evaluate that lesson against the current standards, templates and affected project types. Prefer advisory references for specialized techniques. Version changes to shared obligations, explain adoption in the changelog and preserve existing project pins. Authorized standards maintenance may go directly to main when repository rules permit.
