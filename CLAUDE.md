# Claude Code Instructions

## Pull Requests

- Always create PRs as **draft PRs** by default
- Mark as ready for review only when explicitly requested

### PR Template Auto-fill

When creating PRs, intelligently fill the template:

1. **Summary**: Synthesize from git diff and commit messages - focus on the "why" not just the "what"
2. **JIRA**: Extract ticket key from:
   - Branch name (e.g., `UA-960-some-description`)
   - Commit messages
   - If not found, ask the user
3. **Testing**: Include relevant evidence:
   - If test files were modified → mention specific test coverage added
   - If manually tested → include environment + verification method
   - For API changes → include example requests/responses or logs
   - If version bump/trivial → state "Version bump - no functional changes"
   - **Screenshots/logs required** for any user-visible changes
4. **Checkboxes**: Leave UNCHECKED - human must verify
   - For unit test checkbox: Note if new test files were added or existing tests modified

**Important**: If unsure about any aspect of the PR (JIRA ticket, testing approach, what to include in summary), ask the user before proceeding. Don't guess or make assumptions.

### Special Requirements

- **SDK changes** (FlexActions.Sdk): Note downstream impact on flex-actions-runtime
- **API changes**: Mention if Gateway deployment needed before SDK consumers update
- **Backend changes**: Include verification evidence (logs, API responses, test output)

### Before Creating PR

- Run `/sdlc-workflow:verify-implementation` if a spec exists in `.claude/specs/`
- Verify acceptance criteria from JIRA ticket are met
- Push back if JIRA ticket lacks clear acceptance criteria

## Git Workflow

- Always prompt before committing changes
- Always prompt before pushing changes
- Write descriptive but succinct commit messages

## Testing

- Run `dotnet test` before committing
- Unit tests use xUnit framework
- Each project has a corresponding `.Tests` project
