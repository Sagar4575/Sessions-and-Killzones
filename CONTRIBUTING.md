# Contributing

Contributions, bug reports, and feature suggestions are welcome.

## Reporting a bug

Open an [issue](https://github.com/Sagar4575/sessions-and-killzones/issues) and include:

- Symbol and timeframe where the bug occurs
- A clear description of expected vs. actual behaviour
- A screenshot if relevant

## Suggesting a feature

Open an issue with the `enhancement` label. Describe the use case — that helps evaluate whether it fits the scope of the indicator.

## Submitting a pull request

1. Fork the repository.
2. Create a branch from `main` with a descriptive name:
   - `feat/ny-pm-label-option`
   - `fix/box-right-offset`
3. Make your changes to `fx_market_sessions_with_killzones.pine`.
4. Update `CHANGELOG.md` under `[Unreleased]`.
5. Open a pull request against `main` with a clear summary of what changed and why.

## Code style

The script follows these conventions — please keep them consistent:

| Convention | Example |
|---|---|
| Input variables | `i_sess1_color`, `i_kz1_label` |
| Render functions | `f_render_session()`, `f_render_label()` |
| Helper functions | `f_get_started()`, `f_border_style()` |
| Types | `Session`, `OHLC`, `OpeningRange` (PascalCase) |
| Local variables | `snake_case` |

- Keep render functions focused — one visual responsibility per function.
- Comment any non-obvious logic, especially around bar index math and extend behaviour.

## License

By contributing you agree your changes will be released under the [Mozilla Public License 2.0](LICENSE).
