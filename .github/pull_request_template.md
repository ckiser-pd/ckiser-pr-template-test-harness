<!-- 
This is the flex-actions-library PR template.
Choose the appropriate checklist based on the @releaseLevel of actions you're modifying.

IMPORTANT: Delete the checklist section that doesn't apply to your changes!
-->

## 🔍 Which checklist applies to your changes?

**Check the `@releaseLevel` in your modified action files:**
- Modifying **GA or EA** actions? → Use the **GA/EA Checklist** below, **delete the Development section**
- Working on **Development/Test/Preview** actions? → Use the **Development Checklist** below, **delete the GA/EA section**
- Not sure? Check the `@releaseLevel` JSDoc tag in your `.js` files

---
**📝 Instructions:** Keep only the checklist that applies to your changes and delete the other one.

---

## ✅ GA/EA Action Checklist (Production-Ready)
<!-- Use this section if changing @releaseLevel GA or EA actions -->

**Release Requirements:**
- [ ] My Action uses the correct `@releaseLevel` value (GA or EA)
- [ ] I've used `@featureFlag` if needed to limit access to specific SKU or EA group

**Testing Requirements:**
- [ ] **Unit Tests:** Added/updated `.tests.json` file with comprehensive test coverage
- [ ] **Manual Dev Testing:** Tested action in dev environment with screenshots below
- [ ] **Staging Validation:** Confirmed action works correctly in staging environment
- [ ] **Breaking Changes:** Documented any breaking changes (if applicable) - **If you check this box, please notify the Unified Automation team in #proddev-unified-automation**

### Testing Evidence

**Unit Tests:**
- Test file: `actions/<package>/<action>/<action>.tests.json`
- Tests pass locally: `npm test`

**Manual Testing in Dev Environment:**
<!-- Paste screenshots showing successful execution -->
```
[Screenshot 1: Action configuration]
[Screenshot 2: Successful execution results]
```

**Staging Environment Validation:**
<!-- Confirm the action works in staging -->
```
[ ] Tested successfully in staging
[ ] Verified expected behavior matches dev testing
```

**Breaking Changes:**
<!-- Document any breaking changes, or write "None" -->
```
None
```

---

## ✅ Development Action Checklist (Workshopping)
<!-- Use this section if changing @releaseLevel Development/Test/Preview actions -->

**Release Requirements:**
- [ ] My Action uses the correct `@releaseLevel` value (Development/Test/Preview)
- [ ] I understand this will only deploy to non-production environments

**Testing Status:**
Choose one:
- [ ] Action has `.tests.json` file with test coverage
- [ ] Tests are planned before promoting to GA/EA (see path forward below)
- [ ] This is experimental/prototype work - tests not yet applicable

**Manual Verification:**
<!-- Optional: Describe or show screenshots of any manual testing done -->
```
[Optional: Testing description or screenshots]
```

**Path to GA/EA (if applicable):**
<!-- What needs to happen before this can be promoted to production? -->
```
[Describe the promotion path, or write "N/A - staying in Development"]
```

---

## Summary of Changes
<!-- Describe what you're adding or changing and why -->

**What changed:**

**Why:**

## Feedback Requested
<!-- What specific feedback would you like from reviewers? -->

