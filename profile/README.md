<div align="center">

# OthersJob

**A multi-repository software project with dedicated Quality Assurance, automation and CI/CD practices.**

[![Playwright CI](https://github.com/othersjob/quality-assurance/actions/workflows/playwright-ci.yml/badge.svg)](https://github.com/othersjob/quality-assurance/actions/workflows/playwright-ci.yml)

</div>

---

## Project Structure

| Area | Repository | Purpose |
|---|---|---|
| Quality | [quality-assurance](https://github.com/othersjob/quality-assurance) | QA documentation, test strategy and Playwright automation |
| Frontend | [web](https://github.com/othersjob/web) | Web application interface |
| Backend | [backend](https://github.com/othersjob/backend) | API and service layer |
| Mobile | [mobile](https://github.com/othersjob/mobile) | Mobile application |
| Support | [demo-repository](https://github.com/othersjob/demo-repository) | Demo and experimental repository |

---

## Quality First Approach

The project uses a dedicated QA repository to keep testing assets separated from application code.

The QA layer includes:

- Manual test cases and test plans
- Bug report templates
- API testing documentation
- Risk analysis
- Playwright with TypeScript automation
- GitHub Actions CI/CD

---

## Automation Strategy

Automated tests are maintained in the quality-assurance repository and connect to the applications through URLs and API endpoints.

| Target | Testing Approach |
|---|---|
| web | UI smoke and regression tests |
| backend/API | API checks and integration validation |
| mobile | QA strategy and future mobile automation planning |
| demo-repository | Basic smoke validation where applicable |

This keeps the application repositories clean while allowing independent test execution and reporting.

---

## Tech Stack

| Category | Tools |
|---|---|
| Test Automation | Playwright, TypeScript |
| CI/CD | GitHub Actions |
| API Testing | Playwright Request Context |
| QA Process | Test Plans, Test Cases, Bug Reports, Risk Analysis |
| Documentation | Markdown |

---

## Current Focus

- Stabilizing the Playwright CI workflow
- Expanding smoke and regression coverage
- Improving API test coverage
- Keeping QA documentation aligned with the application repositories

---

<div align="center">

**Built with a focus on software quality, maintainability and test automation.**

</div>