# RabTech Academy - Task 02
## Accessibility Baseline & Repository Architecture Audit

This repository contains my Task 02 work for the RabTech Academy Full Stack Web Development internship.

### Audited website
- Website: https://www.w3.org/
- Audit date: 21 September 2026
- Tool: Lighthouse 13.4.1
- Browser engine: Chromium 153.0.0.0
- Accessibility score: 100/100

### Checks completed
- Lighthouse accessibility audit
- Keyboard-only navigation
- Page structure and semantic landmarks
- Repository architecture and separation of responsibilities

### Repository structure

```text
rabtech-task-02/
├── client/
├── server/
├── docs/
│   ├── accessibility-audit.csv
│   ├── accessibility-report.md
│   ├── architecture.md
│   └── screenshots/
├── tests/
├── .gitignore
└── README.md
```

### Local setup

This task is an architecture skeleton, so there is no application server or database to start yet.

```bash
git clone <repository-url>
cd rabtech-task-02
```

The client and server folders are kept separate so future features can be added without mixing UI, API and documentation code.

### First vertical feature slice

The first planned feature is an accessible dashboard shell covering:
- semantic page layout
- keyboard-friendly navigation
- accessible controls
- client-side data loading
- loading and error states
- basic tests

### Audit note

Lighthouse returned 100/100 for accessibility in this run. The keyboard-only pass also did not show a blocking navigation problem. The report therefore does not invent failed WCAG checks. The documented findings focus on areas that should remain under review as the project grows.
