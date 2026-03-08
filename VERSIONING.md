# Versioning System

## Version Source
- Version is stored in `VERSION` file (format: X.Y.Z)
- Version in `pyproject.toml` must match VERSION file

## Version Bump Rules
- Bump patch version (X.Y.Z -> X.Y.Z+1) for bug fixes
- Bump minor version (X.Y.Z -> X.Y+1.0) for new features
- Bump major version (X.Y.Z -> X+1.0.0) for breaking changes

## CI Requirements
- On push to main branch, VERSION file must be updated
- CI workflow checks that VERSION was bumped on main
- Commit message should include version bump indicator (e.g., "Bump version to X.Y.Z")
