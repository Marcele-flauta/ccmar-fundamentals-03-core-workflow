# Add README Troubleshooting Note

## Problem Statement

The README explains the 5-phase workflow clearly but doesn't address the most common stumbling block new users hit: running `/EA-build` or other commands **before installing the skills**. A short troubleshooting note would reduce confusion.

## Objective

Add a concise "Troubleshooting" section to the README, placed between "Getting Started" and "Quick Reference", containing one practical note about the most common issue.

## Technical Approach

- Edit `README.md` only — no other files change.
- Keep the note short (under 10 lines of markdown) to match the README's existing concise style.
- Use the same formatting conventions already in the file (headings, code blocks, horizontal rules).

## Implementation Steps

### Phase 1: Add Troubleshooting Section

1. Open `README.md`.
2. Insert a new `## Troubleshooting` section **after** the "Getting Started" section (after line 242) and **before** the "Quick Reference" section.
3. Add the following content:

```markdown
## Troubleshooting

**Commands not recognized?**
If `/EA-plan`, `/EA-build`, or other commands aren't available, run `/EA-install` first to install the workflow skills to your project. You can verify they're loaded by checking for a `.claude/commands/` directory in your repo.
```

4. Ensure horizontal rules (`---`) separate it from surrounding sections, consistent with the rest of the file.

## Testing Strategy

- Read the updated README and verify:
  - The new section renders correctly in markdown.
  - It sits between "Getting Started" and "Quick Reference".
  - No existing content was altered or removed.

## Success Criteria

- [ ] A `## Troubleshooting` section exists in the README.
- [ ] It contains one clear, actionable note about missing commands.
- [ ] The surrounding sections and formatting are untouched.
- [ ] The file has no broken markdown.
