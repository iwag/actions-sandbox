# Repository Guidelines

## Project Structure & Module Organization

- Repository root currently contains documentation only.
- `readme.md` is the placeholder project readme.
- `release_flow.md` documents the release candidate workflow for `main` and `release/candidate`.
- No `src/`, `tests/`, or build artifacts are present yet; add new code under a clear top-level directory (e.g., `src/` and `tests/`) and update this guide when introduced.

## Build, Test, and Development Commands

- No build, test, or dev commands are defined in the repository.
- If you add tooling, document it here with concrete examples such as:
  - `npm test` for unit tests
  - `make build` for build artifacts

## Coding Style & Naming Conventions

- No language or formatter is specified.
- Follow the conventions of the language you introduce and keep formatting consistent within each file.
- Prefer clear, descriptive names; keep directory names lowercase and hyphen-free unless a tool requires otherwise.

## Testing Guidelines

- No testing framework is configured.
- When adding tests, choose a framework appropriate to the language and document the command to run tests.
- Use descriptive test names that map to behavior (e.g., `handles-empty-input`).

## Commit & Pull Request Guidelines

- Recent commit messages are short and issue/PR focused (e.g., `Feat/5 (#7)`, `remove template (#3)`).
- Keep commit subjects brief and scoped; include the PR number when applicable.
- Open PRs against `main` and include a concise description of changes and intent.

## Release & Branching Notes

- `main` is the integration branch; `release/candidate` is updated only via the release PR flow.
- Do not commit directly to `release/candidate`; merge to `main` and let automation prepare the release PR.
- See `release_flow.md` for tagging and release steps.
