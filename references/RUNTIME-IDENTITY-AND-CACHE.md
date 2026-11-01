# Runtime identity and cache verification — optional technical recipe

Reference revision 1, 2026-11-01. **Non-normative engineering guidance**, not an amendment to UGDS1.0.0/AICP1.2.1, a new acceptance gate, or adoption of the pending AICP1.2.2 proposal. Use proportionately where local downloadable builds or static-site updates have produced version ambiguity. Existing project pins and owner authority remain unchanged.

## Identify the bytes being reviewed

A source push, a ZIP, a build and a deployed website can have different revisions. Record their relationship instead of calling every latest Git commit the deployed version. One small generated metadata object can supply the footer, build manifest and archive name. An ID based on source/content is more reproducible than a timestamp. Mark uncommitted builds honestly. A documentation-only successor need not rebuild an already accepted runtime; deploy the frozen artifact or establish byte equivalence.

Fingerprint the complete dependency graph, including module imports, dynamic image URLs and styles, rather than only renaming the ZIP. A versioned directory can preserve relative imports without a new bundler. Keep the original editable sources and export recipe; archive names are not browser cache keys.

## Make local updates observable

A local review launcher can send no-store for entry/metadata, and a metadata check can bypass the browser cache. A regular static server controls its own HTTP validators/headers; an already-open tab retains its running JavaScript. Local headers do not configure a hosting provider's CDN. Observe actual public headers and identity before making freshness claims. Keep ordinary TLS verification enabled.

When there was a reported stale build, compare two actual successive packages in the same browser profile and at the same HTTP address. Record the first identity, replace the served artifact, check the old tab, reload, and inspect the new document's resources and identity. Separate late responses from the previous document from resources belonging to the new navigation. Incognito may help diagnose a cache difference; it does not establish the ordinary upgrade path.

## Preserve evidence boundaries

Verify a frozen package's hashes and runtime presence before blaming eligibility or game rules. Exercise real player input and inspect presentation, not just a state flag. Record the exact owner incident as unconfirmed if its file/browser/input sequence was unavailable. A successful new workflow does not prove the old incident's root cause.

For publication, inspect actual deployed identity and canonical asset bytes, then exercise representative live interactions. Successful local tests or a green build alone do not establish a working public destination. Capture physical-device, browser-emulation and human acceptance evidence separately, following existing UGDS/AICP requirements.

## Worked evidence

- [Accepted packaged-build investigation, controlled inputs and same-profile upgrades](https://github.com/jaychtw/shadow-becomes-me/blob/5e26b0c4b521186114d1041a98ccaa3b0cfe7f8d/docs/PLAYTEST_ROUND3.md).
- [Independent canonical public hashes and actual input checks](https://github.com/jaychtw/shadow-becomes-me/tree/ce747118e546c13854b1137270f638e0b2a038a7/evidence/publication/live).

The case's exact earlier owner cache incident remains unconfirmed. This recipe records the demonstrated mitigation/verification method, not a universal cache defect or proof that all projects need this implementation. Core requirements already covered by UGDS-P02/Q04/Q05/Q06 and AICP§4/§6/§7/§10 are not duplicated here. Artifact custody and reasoning escalation remain in the existing unmerged proposal; no parallel proposal is introduced.
