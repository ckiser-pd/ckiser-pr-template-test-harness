## GA/EA Action PR

**This template is for production-ready actions (`@releaseLevel GA` or `EA`).**

---

## Release Checklist
- [ ] My Action uses the correct `@releaseLevel` value (GA or EA)
- [ ] I've used `@featureFlag` if needed to limit access to specific SKU or EA group
- [ ] I've reviewed the [Release Level documentation](https://backstage.pd-staging.com/docs/default/component/flex-actions-library/3a-Release-Properties/)

## Testing Requirements

### Unit Tests
- [ ] Added/updated `.tests.json` file with comprehensive test coverage
- [ ] Tests pass locally: `npm test`
- **Test file location:** `actions/<package>/<action>/<action>.tests.json`

### Manual Testing in Dev Environment
- [ ] Tested action successfully in dev environment
- [ ] Screenshots attached below showing:
  - Action configuration
  - Successful execution
  - Expected outputs/results

**Dev Testing Screenshots:**
```
[Screenshot 1: Action configuration in dev]
[Screenshot 2: Successful execution results]
[Screenshot 3: Output verification]
```

### Staging Environment Validation
- [ ] Action validated in staging environment
- [ ] Behavior matches dev testing expectations
- [ ] No unexpected errors or issues

**Staging Validation Notes:**
```
[Describe staging testing or paste confirmation]
```

## Breaking Changes
- [ ] No breaking changes
- [ ] Breaking changes documented below

**Breaking Change Details (if applicable):**
```
[Document any breaking changes, migration path, or affected workflows]
```

## Summary of Changes

**What changed:**


**Why this change is needed:**


**Impact on existing workflows/users:**


## Feedback Requested

