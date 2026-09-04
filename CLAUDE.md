# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

Starter Express API for the Claude Code course projects.

## Commands
- `npm run dev` - start the API in watch mode (http://localhost:3000)
- `npm test` - run all tests
- `npm run lint` - check code style
- `node --test tests/users.test.js` - run a single test

## Conventions
- Use `node --test` for tests, not external frameworks like Jest or Mocha.
- Put all data access logic in `db/store.js`, not inside route handlers.

## Architecture
- **Entry point**: `server.js` starts the Express API.
- **Routing**: One route file per resource in `routes/`.
- **Data Access**: All data operations are centralized in `db/store.js`.
