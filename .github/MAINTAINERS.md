# Maintainer automation

Community fixture pull requests are handled by GitHub Actions — you do **not** need to approve your own submissions.

## What runs automatically

| Workflow | When |
|----------|------|
| **Fixture PR validate and merge** | PR from branch `fixture/*` or label `fixture-submission` |
| **Fixture issue to PR** | Issue submitted via web form (backup path) |

After checks pass, the **github-actions** bot approves and **squash-merges** the PR.

## One-time repo settings

In **Settings → Actions → General**, under *Workflow permissions*, enable:

**Allow GitHub Actions to create and approve pull requests**

Without this, auto-approve may fail and PRs stay open until merged manually.

## Branch protection (optional)

If `main` has required reviews:

- Allow the **github-actions** bot (or `GitHub Actions`) as an allowed bypass, **or**
- Count bot approvals toward required reviews (default when the setting above is on)

## Re-run a stuck PR

**Actions → Fixture PR validate and merge → Run workflow** and enter the PR number.

## Manual merge

You can still merge by hand if automation fails; read the workflow log for validation errors.
