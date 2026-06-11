<div align="center">

# OthersJob

**A multi-repository software project with a dedicated Quality Assurance and test automation layer.**

[![Playwright CI](https://github.com/othersjob/quality-assurance/actions/workflows/playwright-ci.yml/badge.svg)](https://github.com/othersjob/quality-assurance/actions/workflows/playwright-ci.yml)

</div>

---

## Overview

OthersJob is structured as a multi-repository project, separating application development from quality assurance, test documentation and automation.

The QA strategy is centralized in the [`quality-assurance`](https://github.com/othersjob/quality-assurance) repository, where manual testing artifacts, API testing documentation, Playwright automation and CI/CD workflows are maintained.

---

## Repository Map

| Area | Repository | Purpose |
|---|---|---|
| Quality Assurance | [`quality-assurance`](https://github.com/othersjob/quality-assurance) | QA documentation, test strategy, Playwright automation and CI/CD |
| Frontend | [`web`](https://github.com/othersjob/web) | Web application interface and user flows |
| Backend | [`backend`](https://github.com/othersjob/backend) | API and service layer |
| Mobile | [`mobile`](https://github.com/othersjob/mobile) | Mobile application layer |
| Support | [`demo-repository`](https://github.com/othersjob/demo-repository) | Demo and experimental repository |

---

## QA Architecture

The testing layer is independent from the application repositories.

```text
quality-assurance
├── manual-testing
├── api-testing
├── test-management
├── test-techniques
└── automation-testing
    └── playwright-typescript
```

Automated tests connect to the applications through URLs and API endpoints, without importing or modifying application source code.

---

## Testing Coverage

| Target | Coverage |
|---|---|
| Web | Smoke tests, navigation checks and regression flows |
| Backend/API | Health checks, status validation and API response verification |
| Mobile | QA strategy and future mobile automation planning |
| Demo Repository | Basic smoke validation where applicable |

---

## Quality Practices

- Manual test cases and test plans
- Bug report templates
- API testing documentation
- Risk analysis
- Test management artifacts
- Playwright with TypeScript automation
- GitHub Actions CI/CD
- Test reports and execution artifacts

---

## Tech Stack

| Category | Tools / Practices |
|---|---|
| Test Automation | Playwright, TypeScript |
| CI/CD | GitHub Actions |
| API Testing | Playwright Request Context |
| QA Process | Test Plans, Test Cases, Bug Reports, Risk Analysis |
| Documentation | Markdown |

---

## Current Focus

- Stabilizing the Playwright CI workflow
- Expanding automated smoke coverage
- Improving backend/API validation
- Keeping QA documentation aligned with the application repositories

---

<div align="center">

**Built with a focus on software quality, maintainability and test automation.**

</div>