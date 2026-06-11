# OthersJob

A multi-repository software project with web, backend, mobile and dedicated quality assurance automation.

## Overview

OthersJob is organized as a multi-repository project. Each repository has a specific responsibility, and quality activities are centralized in a separate QA repository.

The goal is to keep application code separated from testing strategy, documentation and automation.

## Repositories

| Repository | Purpose | Main Focus | QA Relevance |
|---|---|---|---|
| `quality-assurance` | Centralized QA repository | Manual testing, API testing, Playwright TypeScript automation and CI/CD | Main repository for test documentation, automation and reports |
| `web` | Web application | Frontend layer and user interface flows | Target for UI smoke and regression tests |
| `backend` | Backend/API services | API and service layer | Target for API validation and integration checks |
| `mobile` | Mobile application | Mobile user experience | Target for mobile QA strategy and future mobile automation |
| `demo-repository` | Demo/support repository | Experiments and project support | Target for basic smoke checks where applicable |

## Architecture

```txt
OthersJob
├── web                 # Frontend layer
├── backend             # API/service layer
├── mobile              # Mobile application layer
├── quality-assurance   # Independent QA documentation and automation layer
└── demo-repository     # Demo/support repository
```

The `quality-assurance` repository is independent from the application repositories.

Automated tests do not import application source code. They connect to running applications through URLs and API endpoints.

## Quality Assurance

The `quality-assurance` repository includes:

- Manual testing documentation
- Test plans
- Test cases
- Bug report templates
- API testing documentation
- Risk analysis
- Test management artifacts
- Playwright with TypeScript automation
- GitHub Actions CI/CD

## Automated Testing

[![Playwright CI](https://github.com/othersjob/quality-assurance/actions/workflows/playwright-ci.yml/badge.svg)](https://github.com/othersjob/quality-assurance/actions/workflows/playwright-ci.yml)

The Playwright automation framework is located in:

```txt
quality-assurance/automation-testing/playwright-typescript/
```

The test strategy covers:

| Area | Approach |
|---|---|
| Web | Smoke and regression testing with Playwright |
| Backend/API | API checks using Playwright request context |
| Mobile | QA strategy and future automation planning |
| Demo repository | Basic smoke validation where applicable |

## CI/CD

The QA workflow is configured in the `quality-assurance` repository.

It is designed to run on:

- Pushes to the main branch
- Pull requests
- Manual execution
- Scheduled daily runs

Reports are generated through Playwright HTML reports and GitHub Actions artifacts.

> Note: The CI status reflects the current state of the automation workflow and may fail while the test environment and required URLs are still being configured.

## Tech Stack

| Area | Tools / Practices |
|---|---|
| Automation | Playwright, TypeScript |
| CI/CD | GitHub Actions |
| API Testing | Playwright request context |
| Manual QA | Test plans, test cases, bug reports, checklists |
| Test Management | Risk analysis, defect management, test monitoring |

## Project Status

This project is being continuously improved with a focus on:

- Software quality
- Maintainability
- Test automation
- Clear documentation
- Separation between application code and QA assets
