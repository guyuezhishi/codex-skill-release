---
name: codex-skill-release
description: Review, package, and publish reusable Codex Skills to GitHub. Use when a user asks to check a skill package, prepare it for sharing, create or update its GitHub repository, or verify a published skill release.
---

# Codex Skill Release

Help the user turn a finished Codex Skill into a clean, usable GitHub repository. Preserve the skill's intended scope and directory layout, remove private or unrelated material, and verify the repository after publishing.

## Workflow

1. **Confirm the release target.** Identify which skill folder and files are in scope, the GitHub owner/repository, and intended visibility. Reuse authorization only for the same files, destination, and visibility. Public exposure requires clear approval for the specific release. Do not infer that a previous public repository authorizes publishing a different skill.
2. **Review the package.** Inspect the full file tree and read the entrypoint, references, scripts, and README. Check frontmatter name/description, references and relative links, scaffold placeholders, and whether each included file supports the skill. Use the skill creator's validator when available. Keep install instructions consistent with the actual layout.
3. **Screen for disclosure and rights issues.** Exclude credentials, tokens, private user data, unrelated project files, private previews, and licensed assets that cannot be redistributed. Inspect absolute paths, personal identifiers, logs, and embedded metadata. A public repository can expose content even when it seems incidental. Do not invent a license or claim that public visibility grants reuse rights; ask the user to choose a license if they want explicit reuse terms.
4. **Package for discovery.** Preserve nested directories exactly. Include a short README for a shared repository with purpose, contents, installation/use, and any material limits. Keep the skill self-contained and avoid publishing archives or generated files unless the user asked for them.
5. **Publish using an available GitHub integration.** Prefer a connected GitHub connector. If unavailable, use the user's already-authenticated browser or an authenticated Git workflow, following the available UI/tool instructions. Never request, copy, print, or store passwords, tokens, or authentication codes. Stop and hand off if authentication or a security challenge requires user action.
6. **Verify the final repository.** Confirm the repository URL and visibility, inspect the file tree and README, check that nested references landed at their intended paths, and confirm the latest commit. If a web upload flattened directories, correct the structure before calling the release complete.
7. **Report clearly.** Provide the repository link, visibility, included files, review results, and any unchosen license or remaining issue. Do not say a release succeeded until the repository itself confirms it.

For a detailed preflight and post-publish checklist, read [references/release-checklist.md](references/release-checklist.md).
