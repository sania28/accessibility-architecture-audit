# RabTech Academy - Task 02

## Accessibility Baseline & Repository Architecture Audit

This repository contains my Task 02 work for the RabTech Academy Full Stack Web Development internship.

## Audited Website

* **Website:** https://www.w3.org/
* **Audit date:** 21 September 2026
* **Tool:** Lighthouse
* **Browser engine:** Chromium
* **Accessibility score:** 100/100

## Checks Completed

* Lighthouse accessibility audit
* Keyboard-only navigation
* Page structure and semantic landmarks
* Repository architecture and separation of responsibilities

## Repository Structure

```text
accessibility-architecture-audit/
├── client/
├── server/
├── docs/
│   ├── accessibility-audit.csv
│   ├── accessibility-report.md
│   ├── architecture.md
│   └── screenshots/
│       ├── lighthouse.png
│       └── keyboard-navigation.png
├── tests/
├── .gitignore
└── README.md
```

## Local Setup

This task is an architecture skeleton, so there is no application server or database to start yet.

```text
git clone https://github.com/sania28/accessibility-architecture-audit.git
cd accessibility-architecture-audit
```

The client and server folders are kept separate so future features can be added without mixing UI, API and documentation code.

## First Vertical Feature Slice

The first planned feature is an accessible dashboard shell covering:

* Semantic page layout
* Keyboard-friendly navigation
* Accessible controls
* Client-side data loading
* Loading and error states
* Basic tests

## Audit Note

Lighthouse returned 100/100 for accessibility in this run. The keyboard-only review also did not identify a blocking navigation problem. The documented findings therefore focus on areas that should remain under review as the project grows.
