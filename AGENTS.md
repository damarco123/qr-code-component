# Agent instructions — qr-code-component

## Issue-bound mockup references (Google Drive + Gigachad)

- Treat every UI mockup as belonging to exactly one GitHub issue in `damarco123/qr-code-component`. Before final Google Drive upload, get the **real issue number**; do not guess it. If no issue exists, request an issue or create one only when authorized.
- Store the asset in `Google Drive/Apps/qr-code-component/` as `issue-<NUMBER>_mockup-v<NN>.<ext>` (for example, `issue-123_mockup-v01.png`). Increment the version on revisions; do not silently overwrite another version.
- Record the exact Google Drive URL **and** `Apps/qr-code-component/<filename>` in the matching issue body or comment. The issue reference, not loose images in a folder, is authoritative for selecting a mockup.
- Coding agents retrieve only the explicitly referenced file using the central rclone connection on Gigachad over SSH, once access is confirmed. Never guess a filename, pick the nearest-looking image, or borrow a mockup from another issue or repo.
- After download, verify repo, issue ID, filename and version against the issue. Only then copy the mockup into the repository's appropriate `contracts/` location if required by that issue and compatible with local project contracts; do not overwrite unrelated references.
- If the issue number, file link, remote access, or match is missing or ambiguous, stop and report the blocker. Do not implement UI changes from an unverified mockup.
- This is an external asset handoff convention; existing repository safety, implementation and contract rules continue to take precedence.
