# MS-4014 repository guidance

## Current course baseline
- The current baseline is the July 2026 major refresh: **Course MS-4014-A: Introduction to building AI agents**.
- Treat the course as exactly **3 current modules (M01–M03)**.
- Use the official module titles exactly as published.
- Do **not** restore old Graph connector, declarative-agent, old lab repo/Pages, or old MS-4014 playlist content into attendee-facing material.

## Audience boundaries
- `README.md` is attendee-facing HackMD content.
- `docs/` is trainer-only and Traditional Chinese; keep technical names and links in English.
- `docs/teaching-guide.md` and `docs/version-change-notes.md` own legacy explanations and migration notes.
- This is a conceptual Microsoft 365 course: do not add Terraform, demo-environment setup, or model/resource provisioning guidance to attendee materials.

## README rules
- Preserve the existing front matter badge/tags/GA values; only `Date`, `Course ID`, and `Course Survey` change per delivery.
- Do **not** add `## Lab`, `## Course Info`, `## Credentials`, or `## Exam & Credential`.
- `## Course` must include the no-hands-on-lab warning.
- Keep the H2 order exact: `Course`, `Course Materials`, `Infos`, `Links`, `Videos`, `What could be next?`, `Mind Map`, `Contact`.
- Use the official Learn path and course page in **EN**, **zh-cn**, and **zh-tw**.
- Use official sources only, and verify links semantically; a 200 response is not enough.
- Keep standalone links separated by exactly one blank line.
- The Mind Map must contain exactly **3 official module nodes** and follow the official module order.
- The front-matter badge image is exempt from the ledger title check.
- Survey and contact entries are per-instance exceptions.

## Videos
- Keep only live, official Microsoft-channel videos that are directly relevant to the module.
- Do not pad with dated or weak clips.
- Remove the section entirely if no good videos qualify.

## Verification
- Build a session-derived link ledger, then run the bundled checker: `.github\skills\course-prep\scripts\link_check.py`.
- Verify final URL, page title, and locale for every document link.
- Do not commit generated ledgers, validation reports, or virtualenv folders.

## Trainer facts to preserve
- The real delivery baseline is the **3-hour Trainer Prep Guide** delivery, not the one-day Learn listing.
- Preserve these teaching-guide facts: **8 literal `Discussion` slides**, **1 M03 `Try it`**, no invented answers for knowledge checks **91/92**, and required terminology updates.

## Repo hygiene
- Keep `.gitignore` and `.gitattributes` focused on transient-file exclusion and consistent text/binary handling.
- Add binary assets only when required, and mark them with the right attributes.
- Use Conventional Commits with the required trailers for commits in this repo.
- Include the required `Co-authored-by` and `Copilot-Session` trailers.
