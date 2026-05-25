# Contributing fixtures

You do **not** need git or to open a pull request yourself.

## From Captivate (recommended)

1. Build and test the fixture in Captivate.
2. Set **Manufacturer** and **Fixture Name**.
3. **Share to Library…** → **Submit to Library**.
4. Sign in to GitHub if prompted (browser), paste JSON if using the web form fallback.
5. A bot opens a pull request for maintainers to review and merge.

## From the web

[Open a fixture submission](https://github.com/NicholasTracy/captivate-fixture-library/issues/new?template=fixture-submission.yml) — paste JSON exported from Captivate.

## File layout (created by the bot)

```
fixtures/{manufacturer-slug}/{model-slug}.json
```

## Pull request checklist (maintainers)

- [ ] Channel map is reasonable and path matches manufacturer/model
- [ ] JSON uses `captivate.fixture-library` schema version 2
- [ ] No duplicate path for the same model

## Optional: one-click submit in Captivate (OAuth)

To enable GitHub Device Flow inside the app (no browser form), register an OAuth App with Device Flow enabled and set the client id in Captivate’s `fixtureLibraryCommunitySubmit.ts`. Until then, submit uses the issue form + clipboard.
