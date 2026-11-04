# Contributing Guidelines

Thank you for your interest in contributing to my projects !

This document defines the general contribution guidelines shared across my personal GitHub repositories.

The goal is to maintain consistent development practices, encourage collaboration, and ensure code quality 
without restricting the technical independence of the individual projects.

Project-specific contribution guidelines take precedence over this document.

## 1. Getting Started

Before contributing :

1. Read the project's `README.md` and relevant documentation.
2. Review existing issues and pull requests to avoid duplicate work.
3. Check the project's development status, roadmap, and technical requirements.
4. For significant changes, consider opening an issue to discuss the proposed approach.
5. Follow any additional instructions provided by the project.

Not all repositories are actively maintained or open to external contributions. Check each project's 
contribution policy before starting substantial work.

## 2. Development Workflow

The recommended contribution workflow is:

1. Fork the repository if you do not have direct write access.
2. Clone the repository locally.
3. Create a dedicated branch from the appropriate base branch.
4. Implement your changes.
5. Run relevant tests and quality checks.
6. Commit your changes using the conventions described below.
7. Push your branch and open a pull request.

Keep changes focused on a single feature, fix, or clearly defined objective whenever possible.

## 3. Branch Naming Conventions

Use descriptive branch names with consistent prefixes.

| Prefix      | Purpose                | Example                      |
|-------------|------------------------|------------------------------|
| `feat/`     | New features           | `feat/elf-loader`            |
| `fix/`      | Bug fixes              | `fix/memory-alignment`       |
| `docs/`     | Documentation          | `docs/kernel-architecture`   |
| `refactor/` | Code Restructuring     | `refactor/event-system`      |
| `test/`     | Tests                  | `test/bootloader-validation` |
| `build/`    | Build system changes   | `build/cmake-configuration`  |
| `ci/`       | Continuous integration | `ci/rust-checks`             |
| `chore`     | Maintenance tasks      | `chore/dependency-update`    |

Use lowercase letters and hyphens to separate words.

Branch names should be concise, descriptive, and relevant to the work being performed.

## 4. Commit Message Conventions

Projects follow the **Conventional Commits** specification.

Commit description are generally written in French, while technical prefixes remain in English.

**Format**

```text
<type>(<scope>): <description>
```

The scope is optional but recommended when it improves clarity.

**Common Commit Types**

| Type       | Description                                              |
|------------|----------------------------------------------------------|
| `feat`     | Introduces a new feature                                 |
| `fix`      | Fixes a bug                                              |
| `docs`     | Updates documentation                                    |
| `refactor` | Restructures code without changing its intended behavior |
| `test`     | Adds or updates tests                                    |
| `build`    | Updates build systems or dependencies                    |
| `ci`       | Updates continuous integration                           |
| `perf`     | Imporves performance                                     |
| `style`    | Changes formatting without affecting behavior            |
| `chore`    | Performs general maintenance                             |

**Examples**

```text
feat(boot): Ajout de la lecture des segments ELF
fix(memory): Correction de l'alignement des pages
docs(kernel): Documentation de l'architecture mémoire
refactor(input): Simplification de la gestion des événements
test(core): Ajout des tests de validation
ci(rust): Ajout des vérifications automatiques
```

**Recommendations**

- Use the nominative form when possible.
- Keep the subject concise and meaningful.
- Avoid vague messages such as `update`, `fix stuff`, or `changes`.
- Separate unrelated modifications into distinct commits.
- Explain complex changes in the commit body when necessary.
- Identify breaking changes using Conventional Commits specification.

## 5. Code Quality

Contributions should prioritize reliability, readability, and maintainability.

General expectations:

- Follow the language-specific conventions used by the project.
- Preserve the existing architecture unless a change has been discussed.
- Avoid unnecessary dependencies.
- Prefer clear abstractions over excessive complexity.
- Handle errors explicitly when appropriate.
- Avoid introducing warnings or regressions.
- Keep implementation details documented when necessary.

**Testing**

Before submitting a pull request:

- Run existing automated tests when available.
- Add tests for new behavior whenever practical.
- Verify bug fixes against the original issue.
- Run relevant formatters, linters, and static analysis tools.
- Document any tests that could not be executed.

Projects involving operating systems, graphics, artificial intelligence, or infrastructure may require
additional validation procedures.

## 6. Pull Requests

Pull requests should clearly communicate that purpose and impact of the proposed changes

**Requirements**

Each pull request should include:

- A concise description of the changes.
- A reference to related issues, when applicable.
- A summary of relevant tests and verification steps.
- Information about breaking changes or compatibility concerns.
- Updated documentation when necessary.

**Review Process**

Code reviews are encouraged, particularly for architectural changes, shared components, and collaborative 
projects.

Reviewers may request modifications before merging.

Approval requirements and branch protection policies are defined individually by each repository.

For collaborative projects, contributors should avoid merging changes that have unresolved critical review
comments.

## 7. Documentation

Documentation is considered part of the development process.

Contributors should update documentation when changes affect:

- Public interfaces or APIs.
- Configuration and installation procedures.
- Architectural decisions.
- User-facing behavior.
- Build and deployment processes.
- Developer workflows.

Public-facing documentation should generally be written in English unless a project explicitly specifies otherwise.

## 8. Security

Do not include credentials, API keys, private certificates, tokens, or other sensitive information in commits, issues, 
or pull requests.

Potential security vulnerabilities should be reported through the project's designed private reporting channel rather
than publicly disclosed before appropriate assessment.

Refer to `SECURITY.md` for additional guidance.

## 9. Project-Specific Requirements

Different projects may use different programming languages, architectures, build systems, and testing strategies.

For example:

- **Northstar OS**: Rust, assembly, UEFI, low-level memory management, and system-level testing.
- **Keystone Engine**: C++, modular engine architecture, graphics, and platform-specific development.
- **The Bloomkeeper**: Gameplay systems, assets, user interaction, and engine integration.
- **Améthée AI**: Machine learning experimentation, reproducibility, and model evaluation.
- **Frosthold**: Infrastructure, deployment, monitoring, and operational security.

Always consult the repository's own documentation before contributing.

## 10. Communication & Collaboration

Constructive collaboration is encouraged.

- Be respectful and professional.
- Provide actionable technical feedback.
- Explain the reasoning behind significant design decisions.
- Ask questions when requirements are unclear
- Keep discussions relevant to the project.
- Respect the time and contributions of other participants.

---

*These guidelines are intended to support consistent, maintainable, and collaborative software development across my
personal projects.*