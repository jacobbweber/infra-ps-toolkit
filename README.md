# infra-ps-toolkit
Infra-PS-Toolkit is a PowerShell module providing admin and automation tools for common IT systems. Includes functions for reporting, troubleshooting, and common infrastructure tasks.

v1.0.1

This project is using:
[Semantic Versioning](https://semver.org/spec/v2.0.0.html).
[Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/).
[Keep a Changelog](https://keepachangelog.com/en/1.1.0/).
Changes are documented in [CHANGELOG.md](CHANGELOG.md).

## Branching Strategy

    - Pull Requests require at least one approval and successful build.
    - Merges to main trigger a release build and publish to local build endpoint.**
    - Releases are tagged with the version number.
    - Pre-release versions are tagged with -alpha, -beta, or -rc.
    - Commits to main must be signed.
    - CI/CD is done with GitHub Actions.
    - Code reviews are required for all changes to main.
    - Issues and PRs must reference a work item in the project management tool.
    - Automated tests are required for all new features and bug fixes.
    - Documentation must be updated for all changes to functionality.
    - Security scans are run on all code changes.

>Note: **(TBD Based on Future lab)

## Commit Message Guidelines

**build**: Changes that affect the build system or external dependencies (example scopes: gulp, broccoli, npm)
**ci**: Changes to our CI configuration files and scripts (example scopes: Travis, Circle, BrowserStack, SauceLabs)
**docs**: Documentation only changes
**feat**: A new feature
**fix**: A bug fix
**perf**: A code change that improves performance
**refactor**: A code change that neither fixes a bug nor adds a feature
**style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
**test**: Adding missing tests or correcting existing tests
**chore**: Changes to the build process or auxiliary tools and libraries such as documentation generation
**revert**: Reverts a previous commit
BREAKING CHANGE: A commit that introduces a breaking API change

Examples:
- feat: add new user login feature
- fix: correct typo in README
- docs: update API documentation for new endpoints
- style: reformat code with prettier
- refactor: simplify user authentication logic
- perf: improve database query performance
- test: add unit tests for user service
- chore: update dependencies to latest versions
- ci: add GitHub Actions workflow for CI/CD
- build: update webpack configuration for production build
- revert: revert "feat: add new user login feature"

- Breaking Change examples:
  - feat!: overhaul authentication system (BREAKING CHANGE)
  - fix!: remove deprecated API endpoint (BREAKING CHANGE)
  - refactor!: change database schema (BREAKING CHANGE)
  - perf!: optimize image processing algorithm (BREAKING CHANGE)
  - ci!: change CI provider (BREAKING CHANGE)
  - build!: switch to new build tool (BREAKING CHANGE)
  - style!: enforce new code style guidelines (BREAKING CHANGE)
  - revert!: revert "refactor!: change database schema" (BREAKING CHANGE)
  - BREAKING CHANGE: change API response format (BREAKING CHANGE)
  - feat: add support for new authentication method