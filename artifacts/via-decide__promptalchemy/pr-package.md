Branch: simba/fix-pipeline-failure-by-ensuring-only-a-md-task-
Title: Fix pipeline failure by ensuring ONLY a .md task file is generated an...

## Summary
- Repo orchestration task for via-decide/promptalchemy
- Goal: Fix pipeline failure by ensuring ONLY a .md task file is generated and written to disk, preventing missing artifact errors for JS files

## Testing Checklist
- [ ] Run unit/integration tests
- [ ] Validate command flow
- [ ] Validate generated artifact files

## Risks
- Prompt quality depends on repository metadata completeness.
- GitHub API limits/token scope can block deep inspection.

## Rollback
- Revert branch and remove generated artifact files if workflow output is invalid.