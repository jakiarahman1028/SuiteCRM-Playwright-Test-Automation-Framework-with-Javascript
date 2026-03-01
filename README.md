# SuiteCRM Playwright Automation Framework

End-to-end automation framework built using:
- JavaScript
- Playwright
- Page Object Model (POM)
- CI/CD Ready Architecture

---

## 📌 Project Objective

This framework automates the following SuiteCRM modules:

- Login / Logout
- Create New Account
- Edit Profile

The framework is designed to be:

- Scalable
- Reusable
- Maintainable
- CI/CD Ready

---

## 🏗 Architecture Overview

The framework follows layered architecture:

tests → page objects → base layer → utilities → config

This ensures:
- No duplication
- Clear separation of concerns
- High maintainability

---

## 📁 Project Structure

tests/
    auth/
    account/
    profile/

pages/
    base/
    auth/
    account/
    profile/

fixtures/
utils/
config/

---

## 🔹 Framework Design Principles

1. No test logic inside page files
2. No hardcoded test data
3. Common methods centralized in BasePage
4. Feature-wise test separation
5. Environment-based configuration
6. CI-ready execution

---

## 🚀 Installation

Clone repository:

`git clone <repo_url>`

Install dependencies:

`npm install`

Install Playwright browsers:

`npx playwright install`

---

## ▶ Run Tests

Run all tests:

`npx playwright test`

Run specific module:

`npx playwright test tests/auth`

Run smoke tests:

`npx playwright test --grep @smoke`

Run in headed mode:

`npx playwright test --headed`

---

## 🧪 Test Strategy

Tests are divided into:

- Smoke
- Regression
- Feature-based execution

---

## 🔐 Environment Configuration

Environment variables are stored in:

`config/env.js`

To change environment:

Set ENV variable before execution.

---

## 📊 Reporting

Playwright HTML report:

`npx playwright show-report`

Reports are generated after each execution.

---

## 🔄 CI/CD Integration

GitHub Actions pipeline is configured under:

` .github/workflows/playwright.yml `

Pipeline performs:

- Dependency installation
- Browser installation
- Test execution
- Report artifact upload

---


