[architecture.md](https://github.com/user-attachments/files/32507701/architecture.md)
# Project Architecture

## Overview

This repository uses a simple monorepo-style structure to keep frontend code, backend code, documentation and tests separate.

```text
rabtech-task-02/
├── client/
├── server/
├── docs/
└── tests/
```

## Folder boundaries

### client/

Frontend boundary.

Contains:
- HTML/UI
- CSS
- JavaScript
- client-side state
- API client

Backend and database code should not be placed here.

### server/

Backend boundary.

Contains:
- REST API
- validation
- business logic
- data access

UI-specific code should not be placed here.

### docs/

Documentation and audit material.

Current documentation includes:
- accessibility audit CSV
- accessibility report
- architecture notes
- screenshot evidence instructions

### tests/

Testing boundary.

Future tests can cover:
- keyboard navigation
- UI behaviour
- API responses
- validation
- loading and error states

## Local setup

This repository is currently a skeleton, so there is no build command or database setup.

```bash
git clone <repository-url>
cd rabtech-task-02
```

Future package files can be added inside `client/` and `server/` without changing the main architecture.

## First vertical feature slice

The first planned slice is an **Accessible Dashboard Shell**.

```text
User
  ↓
Client UI
  ↓
API Client
  ↓
Server/API
  ↓
Business/Data Layer
  ↓
Response
  ↓
Accessible UI update
```

The slice will include:
1. Semantic page layout
2. Keyboard-friendly navigation
3. A small API endpoint
4. Loading and error states
5. Basic tests
6. Documentation update

This gives the project one complete feature before additional screens are added.
