# Contributing to SoundSwitch

Thanks for taking a look. SoundSwitch is a small focused tool, so the bar for a
contribution is low: a well-scoped change with a short description beats a
sprawling patch every time.

## Ways to help

- **Report a bug.** Open an issue with your Windows version, the exact steps,
  and (if the app crashed) the latest log file from `%LOCALAPPDATA%/soundswitch/logs`.
- **Propose a feature.** Describe the problem first, the proposed solution
  second. Features that solve a real workflow land faster than features that
  sound neat.
- **Send a pull request.** Fork, branch, commit, open a PR against `main`.
  Please keep the diff focused on one thing.

## Local setup

1. Clone the repository.
2. Install the toolchain listed in the README under *Build from source*.
3. Run the project's `scripts/dev.ps1` to set up dependencies.
4. Build with `scripts/build.ps1` and run the result from `./dist`.

## Code style

- Keep public API names stable; prefer additive changes over renames.
- One logical change per commit; squash fix-up commits before you push.
- Match the surrounding style; this repository does not use autoformatters that
  disagree with the house formatter.
- Tests live next to the code they cover. Add one when fixing a bug so the bug
  cannot come back silently.

## Pull request checklist

- [ ] The change builds locally without new warnings.
- [ ] Existing tests pass and new behavior has a test.
- [ ] User-facing changes are mentioned in `CHANGELOG.md`.
- [ ] If the UI changed, attach a short screen capture or a before/after image.
- [ ] The PR description explains the *why*, not just the *what*.

## Reporting a security issue

Please do not open a public issue for security problems. Email the maintainer
listed in the repository description with a short write-up. Expect an
acknowledgment within three working days.

## Code of conduct

Participation in this project is covered by the [Code of Conduct](code_of_conduct.md).
