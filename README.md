# Captivate Community Fixture Library

Native [Captivate 2](https://github.com/NicholasTracy/captivate-2) fixture definitions shared by the community.

## Browse in Captivate

**Fixtures → Add → Search For Fixture Online → Captivate Community Library**

Filter by manufacturer, then model; import adds the definition to your project.

## Contribute

See [CONTRIBUTING.md](./CONTRIBUTING.md).

Quick path from Captivate:

1. Edit your fixture (manufacturer + model name required).
2. **Share to Library…** → export JSON.
3. Open a pull request adding the file under `fixtures/{manufacturer}/{model}.json`.

## Layout

```
fixtures/
  {manufacturer-slug}/
    {model-slug}.json
```

Use lowercase slugs with hyphens (e.g. `chauvet/colorado-solo.json`).

Each JSON file is a Captivate fixture library document (`schema`: `captivate.fixture-library`, `version`: `2`).

## License

Contributions are accepted under the same license as this repository (see LICENSE). Only submit fixtures you have the right to share.
