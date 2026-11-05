# Playwright Automation

A small Playwright Test project with browser tests in JavaScript.

## What's included

- `tests/UIBasicsTest.spec.js` checks the Playwright homepage title and the Get started navigation.
- `tests/SelectorsTest.spec.js` exercises selectors and filtering in a TodoMVC app.
- `tests/login.spec.js` exercises a login flow using the Page Object Model in `pages/login.js`.

## Prerequisites

- Node.js and npm

## Setup

Install the project dependencies and the Chromium browser used by the tests:

```bash
npm ci
npx playwright install chromium
```

## Run the tests

Run all tests:

```bash
npx playwright test
```

Run a specific test file:

```bash
npx playwright test tests/SelectorsTest.spec.js
```

Run the login test:

```bash
npx playwright test tests/login.spec.js
```

Open the HTML report after a run:

```bash
npx playwright show-report
```

Tests are stored in `tests/` and use the `*.spec.js` naming pattern. The browser and other test settings are in `playwright.config.js`.
