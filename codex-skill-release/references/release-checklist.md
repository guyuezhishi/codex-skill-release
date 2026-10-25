# GitHub Skill release checklist

Use this checklist when the release involves multiple files, a new repository, or a public audience. Skip items that do not apply.

## Before publishing

- Confirm the source skill folder and the exact files the user wants shared.
- Confirm repository owner/name and visibility. Treat public visibility as a separate, consequential choice when it has not been explicitly approved for this release.
- Read `SKILL.md` and every referenced resource. Confirm the skill has a valid YAML frontmatter block, a concise trigger description, no unfinished TODO scaffold, and accurate paths.
- Run the available skill validator, such as `quick_validate.py`, and review its output. Validation checks structure; it does not replace reading the content.
- Check that examples, names, URLs, file paths, screenshots, and metadata do not expose private project details or user information.
- Check that included images, fonts, code samples, and other assets are original, user-provided for redistribution, or licensed for the intended use. Preserve required notices. Do not select a license on the user's behalf.
- Keep the intended folder tree. Include only the README or other package docs that help users install and use the skill.

## During publication

- Prefer the connected GitHub integration when it supports the requested work; otherwise use the authorized authenticated path available in the environment.
- Do not put credentials in commands, files, commit messages, or chat. Let the user handle sign-in challenges, CAPTCHA, or credential entry when the interface requires their direct action.
- For a browser upload, select only the reviewed files. Verify nested paths after upload; some upload pages place every selected file in the repository root.
- Use a factual commit message. Do not add a license unless the user chose one.

## After publishing

- Open the repository and verify its URL, owner, visibility, latest commit, and top-level file list.
- Open each key file or inspect the tree to confirm nested references were preserved and README links resolve.
- Check that no unexpected files, archives, previews, or duplicate misplaced copies were added.
- Report the public/private status and explain if no license is present: visibility alone does not state reuse terms.
