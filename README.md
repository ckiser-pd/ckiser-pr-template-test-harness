# PR Template Test Harness

This is a test repository to validate PR templates for flex-actions-library before merging to main.

## Purpose

Test the PR template structure and content to ensure:
- Templates load correctly in GitHub web UI
- Instructions are clear
- Checklists are appropriate for GA/EA vs Development actions

## PR Templates

- `.github/pull_request_template.md` - Default template (auto-loads)
- `.github/PULL_REQUEST_TEMPLATE/ga-ea-action.md` - Strict template for production actions
- `.github/PULL_REQUEST_TEMPLATE/development-action.md` - Relaxed template for experimental work

## Testing Instructions

1. Create a test branch
2. Make a small change (e.g., add a line to this README)
3. Create a PR and review the template
4. Provide feedback on clarity, completeness, and usability

## Related

- UA-961: Establish PR review standards for flex-actions-library
- Main PR: https://github.com/PagerDuty/flex-actions-library/pull/3118
