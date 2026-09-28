# Changelog — `toxi-config`

Per-crate history extracted from the monolith changelog
([meshackbahati/toxi](https://github.com/meshackbahati/toxi/blob/main/CHANGELOG.md)),
which remains the full documentation hub.

## 3.1.5

- **toxi-config** (`3.1.1`): fixed a self-deadlock in the test helper that
  locked the non-reentrant `SERIAL_TEST` mutex while callers already held
  it, which hung the config suite indefinitely. Test-only change.
