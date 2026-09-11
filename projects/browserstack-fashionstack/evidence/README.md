# FashionStack Hackathon Evidence Index

This folder preserves recovered artifacts and live BrowserStack evidence from Ashley Cichy's 2026 BrowserStack AI Hackathon submission in the E-Commerce track.

## Mission 01: The AI Test Architect

**Official requirement:** Generate/refine a manual test suite from the FashionStack user stories, push at least two cases into Low Code Automation, execute the generated automation, and submit both a Test Management CSV export and a public successful LCA build.

**Recovered evidence:**

- [`mission-01-test-management-export.csv`](./mission-01-test-management-export.csv) - recovered BrowserStack Test Management export containing TC-300 and its detailed steps, expected results, project metadata, and AI refinement prompt. The prompt documents the 16-case structure across US-01 through US-04.
- BrowserStack Test Management case URL preserved inside the CSV for TC-300.

## Mission 02: Mastering Data & Enterprise Workflows

**Official requirement:** Build two login -> action -> logout workflows using a reusable `Login` module, reusable `Logout` module, shared `UserEmail` global variable, and encrypted `LoginPassword` secret. Both tests had to pass, and the submission required a public build plus a screenshot showing the global variable USED IN count across multiple tests.

**Recovered evidence:**

- [Public BrowserStack M02 build](https://low-code.browserstack.com/projects/4020759/builds/ytmqporhxmztcmrvt85rxaeovoo9graunciiswff?public_token=050912ea5a7e3216116e481201f3f9d621b193b7288696c8ae5ae8bf7b1c782f)
- Build name: `M02 - FashionStack Enterprise Workflows-6`
- Passing test: `M02 - Login, Add to Cart, and Logout`
- Passing test: `M02 - Login, Verify Men Inventory, and Logout`

## Mission 04: The Resilient Pipeline

**Official requirement:** Establish a passing login baseline, intentionally change the locator target, confirm the unchanged test fails, enable AI Self-Healing, rerun the same test, and verify the healed locator / Self-Healed indicator in the execution history.

**Recovered evidence from the original project history:**

- `M4 AI Self Healing-1` - passed on Aug 13, 2026 at 12:26:55 AM EDT.
- `M4 AI Self Healing-2` - failed on Aug 13, 2026 at 12:43:47 AM EDT.
- The failed execution shows the step `Hover over "Back to Home" button` with the error `Could not find element on the page`.
- `M4 AI Self Healing-3` - passed on Aug 13, 2026 at 12:46:18 AM EDT.

The recovered screenshots preserve the pass -> locator failure -> subsequent pass sequence. The currently accessible BrowserStack account view does not expose the original public self-healed session token, so this portfolio does not present a currently verifiable public Self-Healed badge link.

## Mission 05: Test Case Mapping and Results Sync

**Official requirement:** Map Low Code Automation tests to BrowserStack Test Management case IDs, execute the mapped tests, export the XML report from the build, upload the result into Test Management, and submit both a Test Management run screenshot and the exported XML report.

**Recovered evidence:**

- [Public BrowserStack M05 build](https://low-code.browserstack.com/projects/4024697/builds/rfjctl2wtr2solhyvcnahd4jmvtbrnygswrahtuy?public_token=ab46fe7fc2f4b17a7941c190b95981701d8eb1784109c61ebf5651c17becea1b)
- [`mission-05-tcm-results.xml`](./mission-05-tcm-results.xml) - original-style JUnit XML evidence with 2 tests, 0 failures, and mapped IDs `TC-300` and `TC-301`.
- Recovered Test Management run: `M05 - FashionStack LCA Results Sync #1`, created by Ashley Cichy on Aug 13, 2026, 2 tests, 2m 49s, 2 passed, 0 failed, no failures.
- Recovered Project Insights view: 16 total test cases, 14 manual test cases, 2 automated test cases, and 12.50% automation coverage.

## Why these artifacts matter

Together, the recovered evidence shows the project moving from requirements and AI-assisted manual test design into reusable low-code automation, locator-failure recovery, and automation-to-Test Management traceability. BrowserStack later recognized the submission as the cleanest four-mission entry in the competition and specifically praised the documentation, TC-300 / TC-301 XML reporting, and verified Low Code Automation public build links.
