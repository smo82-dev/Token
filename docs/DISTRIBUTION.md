# Public distribution and release policy

This public repository `smo82-dev/Token` is for approved Flipper release downloads, short release notes, checksums and public-facing documents. The private `smo82-dev/Flipper` repository is the authoritative source for implementation and build verification.

## Release gates

1. Build and test in the private source repository. Record the source revision, application version, build provenance and Windows test results.
2. Confirm the Windows installer includes the native host, has appropriate publisher/signing status, and has passed the owner's manual acceptance. The published Chrome Web Store extension must actually support any desktop-connect instructions shown to consumers.
3. Obtain explicit owner approval for the specific version and exact file digests.
4. Prepare a GitHub Release in this public repository, with version tag `vX.Y.Z`, versioned installer, SHA-256 checksums, concise release notes and support links. Pre-release builds must be conspicuously marked as such.
5. Verify the public download, installer file hash, version, and link from Chrome onboarding. Do not advertise an unapproved package as production.
6. Keep old approved versioned releases available when practical. Do not silently swap binaries attached to an existing release.

## Public asset boundary

Only distribute approved installers and public documentation. Do **not** copy private Git history or source, build credentials, API keys, signing/private keys, authentication tokens, raw user data, sensitive diagnostics or full internal workflow logs.

Prefer a dedicated narrowly scoped GitHub App or fine-grained token with permission to write releases only to Token. Never embed credentials in a public workflow or commit. Protect publishing behind an owner-controlled release environment/approval process. Default workflow `GITHUB_TOKEN` should remain read-only.

## Release link strategy

Browser onboarding should point to the stable public Releases page `https://github.com/smo82-dev/Token/releases` until a verified stable release-download routing strategy is ready. Do not hard-code short-lived Actions artefact links or a version-specific asset without maintaining updates.

## Administrative settings to confirm (not changed by this document)

- Keep repository **public** and default branch **main**; leave the name **Token** unchanged.
- Configure branch rules for `main` appropriate to the account's GitHub plan; at minimum require PR review where available and block force pushes and branch deletion.
- Enable Dependabot alerts and secret scanning where available.
- In Actions > General, allow only required actions and retain read-only default workflow permissions.
- Disable unused Wiki/Projects/Discussions if desired; decide whether public Issues should remain available for support.
- Require explicit release approval; do not turn on automatic publication from pushes or merges.

**No release workflow, tag, release or installer has been published by this documentation change.** A gated release pipeline must be designed and tested with authorised credentials before automation is enabled.
