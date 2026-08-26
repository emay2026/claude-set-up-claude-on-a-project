# Project Setup Notes

## CLAUDE.md
I included essential development commands, architectural patterns (like centralized data access in `db/store.js`), and the project entry point. I deliberately left out granular implementation details and boilerplate setup because those can be discovered through code exploration; `CLAUDE.md` is intended for high-level guidance and project-specific idioms.

## Permission Rules
I added rules to allow `npm test`, require confirmation for `git push`, and explicitly deny reading `.env` and using `git push --force`. Without the deny rules, the agent could accidentally leak sensitive secrets from the `.env` file or catastrophically overwrite the remote git history with a force push.
