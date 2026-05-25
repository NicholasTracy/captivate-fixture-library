# Captivate Community Fixture Library

Community-built [Captivate 2](https://github.com/NicholasTracy/captivate-2) fixture definitions—ready to import by manufacturer and model.

## Use fixtures in Captivate

1. **Fixtures** → **Add** (+) → **Search For Fixture Online**
2. **Source:** **Captivate Community Library**
3. Choose **manufacturer** → **model** → **Import**

Also available in the same dialog: **QLC+ Fixture Library** and **Open Fixture Library**.

## Submit a fixture

You do **not** need git or to open a pull request.

### From Captivate (recommended)

1. Build and test your fixture; set **Manufacturer** and **Fixture Name**.
2. **Share to Library…** → **Submit to Library**
3. Sign in to GitHub when prompted, then confirm in Captivate.
4. The library bot validates and merges your pull request automatically (no self-approval needed).

See [CONTRIBUTING.md](./CONTRIBUTING.md) for details and the web-only path.

## Repository

Fixtures live under `fixtures/{manufacturer}/{model}.json`. New submissions are validated by GitHub Actions and merged when checks pass.

## License

Contributions are under the license in [LICENSE](./LICENSE). Only share fixtures you have the right to distribute.
