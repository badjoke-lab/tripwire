# Agent Instructions

This repository follows specific safety and operational rules for coding agents. Agents must adhere to these guidelines to maintain the project's defensive and educational mission.

## Core Procedures

1.  **Read Context First**: Always read `README.md` and relevant documentation in `docs/` before proposing or implementing changes.
2.  **Verify Status**: Do not rely solely on roadmap numbering or stale status files. Inspect the current codebase to determine the actual state of implementation.
3.  **Atomic Pull Requests**: Keep pull requests focused with one clear purpose. Avoid unrelated refactoring or scope creep.
4.  **Minimal Changes**: Prefer minimal, reversible changes. Do not expand scope without explicit approval.

## Safety and Content Boundaries

5.  **Defensive Mission**: Preserve the project's focus on defensive safety and developer education.
6.  **No Offensive Material**: Never add exploit steps, attack instructions, bypass methods, credential theft methods, weaponized payloads, evasion instructions, or other offensive operational details.
7.  **Fact-Checking**: Never publish unverified claims as facts.
8.  **Data Separation**: Keep candidate and review data (e.g., `data/*.example.json`, `data/manual-intake.json`) separate from published card data (`data/threats.json` and `data/threats-approved.json`).
9.  **No Auto-Publishing**: Never implement logic that automatically publishes candidate content to the public site.
10. **Semantic Preservation**: Preserve source links and confidence/freshness/severity semantics when modifying data or related logic.

## Technical Standards

11. **Cross-Language Verification**: When changing shared user-facing behavior, verify both English and Japanese (`/ja/`) surfaces.
12. **Mandatory Validation**: Run `npm run check` before completing any code or data changes.
13. **Local Validation**: Run any additional relevant validation scripts (e.g., `npm run time-policy:check`, `npm run ai-output:validate`) if working in those specific areas.
14. **Accurate Reporting**: Report validation results accurately. Never claim checks passed if they were not run successfully.
15. **Neutral PR Descriptions**: PR descriptions must be neutral and technical, using:
    - **Summary**: What was changed.
    - **Validation**: How it was tested.
    - **Out of Scope**: What was intentionally left out.
16. **Privacy**: Do not expose secrets, local files, credentials, private notes, or untracked operator data in commits or PR descriptions.
17. **No Auto-Merge**: Do not merge pull requests automatically unless explicitly instructed.
18. **Report Conflicts**: When documentation conflicts with the actual implementation, investigate and report the conflict rather than assuming either side is correct.
