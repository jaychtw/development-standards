# Runtime identity and cache verification — optional technical recipe

**Status:** Non-normative engineering reference, adapted from PR #8 (originally 2026-11-01). This is **not** a mandatory new UGDS/AICP gate or an explanation proven for every cache-related bug. Apply selectively to static sites, local downloadable builds, artifacts or deployments where revision identity is materially uncertain.

## Identify what is actually running

A source commit, ZIP, packaged output, CI artifact, deploy revision and browser document can have different identities. Record their relationship only when needed; a single machine-generated manifest or build-info file can serve several purposes. Content-based identification is often more reproducible than timestamps. Mark builds with uncommitted files honestly. A documentation-only commit need not rebuild a previously accepted runtime merely to change its version label.

Fingerprint the **complete runtime asset dependency graph** (entry HTML, imported modules, dynamic images and styles) where cached mismatches are a realistic risk; changing only a ZIP filename is not cache invalidation. Preserve editable inputs and reproducible export commands. A versioned asset directory can preserve relative imports without requiring another bundler.

## Test actual upgrade behavior when justified

A local review server can use no-store for entry/metadata, and a direct metadata request can bypass browser caches for diagnosis. Local server headers do **not** establish the deployed host/CDN's caching policy. An already-open tab retains its old code until it updates or reloads. Inspect the actual deployed response headers and canonical asset identity; do not disable ordinary TLS validation.

When stale builds are suspected, test two successive **actual** packages at the same URL in the **same browser profile**: record version A; replace the served artifact with B; observe existing tab, reload, inspect the new document's resources and identify B. Distinguish late responses belonging to A from B's requests. Incognito can isolate a suspected cache influence but does not verify the normal upgrade path.

## Evidence and limitations

Confirm the frozen package exists, its expected bytes match and actual controls respond before attributing a failure to game logic, browser caching or release promotion. Separate source, build, browser, user input and deployed identity evidence. Green CI is not proof of the public live result. Automated checks and human/physical-device observation have different evidence status under the adopted standards; do not invent owner acceptance.

**Observed case references:**
- [Shadow Becomes Me controlled-input and same-profile update investigation](https://github.com/jaychtw/shadow-becomes-me/blob/5e26b0c4b521186114d1041a98ccaa3b0cfe7f8d/docs/PLAYTEST_ROUND3.md)
- [Independent public hash and input checks](https://github.com/jaychtw/shadow-becomes-me/tree/ce747118e546c13854b1137270f638e0b2a038a7/evidence/publication/live)

The exact root cause of the earlier reported owner cache incident was **not confirmed**. These examples demonstrate possible verification techniques, not a universal caching flaw. For routine releases use the project's agreed checks and AICP's release verification; **do not run this expanded procedure unless revision/cache ambiguity warrants it**.
