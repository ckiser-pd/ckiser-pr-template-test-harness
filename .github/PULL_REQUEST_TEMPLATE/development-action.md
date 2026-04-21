## Development Action PR

**This template is for experimental/workshopping actions (`@releaseLevel Development`, `Test`, or `Preview`).**

---

## Release Checklist
- [ ] My Action uses the correct `@releaseLevel` value (Development/Test/Preview)
- [ ] I understand this will only deploy to non-production environments
- [ ] I've reviewed the [Release Level documentation](https://backstage.pd-staging.com/docs/default/component/flex-actions-library/3a-Release-Properties/)

## Testing Status

**Select the option that applies:**
- [ ] **Option A:** Action has `.tests.json` file with test coverage
- [ ] **Option B:** Tests are planned before promoting to GA/EA (see path forward below)
- [ ] **Option C:** This is experimental/prototype work - formal tests not yet applicable

**Test Details (if Option A):**
```
Test file: actions/<package>/<action>/<action>.tests.json
Tests pass: [ ] Yes  [ ] No (explain below)
```

## Manual Verification

**Manual testing performed:**
<!-- Optional but encouraged: Describe testing done or attach screenshots -->
```
[Describe what manual testing you did, if any]
[Optional: Screenshots showing it works]
```

## Path to GA/EA (if applicable)

**Is this action intended for production eventually?**
- [ ] Yes - planning to promote to GA/EA
- [ ] No - staying in Development for internal/experimental use
- [ ] Undecided

**If yes, what needs to happen before promotion:**
```
[ ] Add comprehensive .tests.json coverage
[ ] Complete manual testing in dev
[ ] Validate in staging
[ ] Get security/compliance review (if needed)
[ ] Documentation complete
[ ] Other: ___________
```

## Summary of Changes

**What changed:**


**Why:**


**Current limitations or known issues:**


## Feedback Requested

