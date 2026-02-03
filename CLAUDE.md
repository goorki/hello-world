# CLAUDE.md

This file provides guidance for AI assistants working with this repository.

## Repository Overview

**hello-world** is a starter repository. Currently minimal, it serves as a foundation for future development.

### Current Structure

```
hello-world/
├── README.md      # Project description and documentation
├── CLAUDE.md      # AI assistant guidelines (this file)
└── .git/          # Git version control
```

## Development Guidelines

### Git Workflow

1. **Branching**: Create feature branches from the main branch
2. **Commits**: Write clear, descriptive commit messages
3. **Pull Requests**: Submit PRs for code review before merging to main

### Commit Message Format

Use conventional commit style:
- `feat:` for new features
- `fix:` for bug fixes
- `docs:` for documentation changes
- `refactor:` for code refactoring
- `test:` for adding tests

Example: `feat: add user authentication module`

## For AI Assistants

### When Working on This Repository

1. **Read before modifying**: Always read existing files before making changes
2. **Keep it simple**: Avoid over-engineering; make only necessary changes
3. **Document changes**: Update README.md when adding significant features
4. **Test changes**: Verify modifications work before committing

### File Conventions

- Use lowercase with hyphens for filenames (e.g., `my-feature.js`)
- Keep the repository structure flat unless complexity requires folders
- Include appropriate file extensions

### What to Avoid

- Do not add unnecessary dependencies
- Do not create files without clear purpose
- Do not modify this CLAUDE.md without user request
- Do not commit sensitive information (API keys, credentials)

## Future Development Notes

As this repository grows, update this file with:
- Build and test commands
- Environment setup instructions
- Architecture decisions
- Code style guidelines specific to the chosen tech stack
