# BrowserStack AI Hackathon — Fashion Stack E-Commerce QA Project

## Ashley Cichy | QA Engineer & Computer Science Student

**Achievement:** 2nd Place Winner — E-Commerce Track  
**Demo Application:** https://ecommercebs.vercel.app/  
**Platform:** BrowserStack Test Management + Low Code Automation

## Project Overview

I completed four qualifying technical missions for BrowserStack's Fashion Stack e-commerce challenge. The project combined AI-assisted test design, manual test management, low-code automation, reusable test architecture, secure test data handling, AI self-healing, and automated-results traceability.

BrowserStack's evaluation team recognized the submission as the **cleanest four-mission submission in the entire competition**, specifically praising the thorough documentation, multi-testcase XML reports **TC-300** and **TC-301**, and verified Low Code Automation public build links.

### Core Skills Demonstrated

- Test case design from user stories and acceptance criteria
- Positive, negative, boundary, and edge-case coverage
- BrowserStack Test Management and Low Code Automation
- AI Test Case Generator and Low-Code Authoring Agent workflows
- Reusable Login and Logout modules
- Global variables and encrypted secrets
- Cloud-based automated test execution
- AI-powered locator self-healing
- XML/JUnit-style test-result reporting
- Automation-to-test-case traceability

---

## Mission 01 — The AI Test Architect
### TCM and LCA Generation

**Goal:** Convert product user stories into a structured manual test suite, then turn selected cases into automated Low Code Automation workflows.

### User Stories Covered

- **US-01 — Homepage Hero Carousel:** Verify dynamic carousel behavior, including normal transitions and interaction stability.
- **US-02 — Men's Category Inventory:** Verify the Men's category displays the expected inventory of **16 products**.
- **US-03 — Cart Counter:** Verify Add to Cart actions update the persistent cart counter correctly.
- **US-04 — Authentication:** Validate login behavior across successful, negative, and edge-case scenarios.

### What I Completed

- Created a BrowserStack Test Management project for the Fashion Stack application.
- Used BrowserStack's AI Test Case Generator to generate test cases from the supplied user stories.
- Reviewed and refined AI-generated cases so the suite included core paths, negative scenarios, and edge cases rather than relying only on happy-path coverage.
- Built carousel scenarios that included automatic transition behavior, rapid-click stability, and missing/broken-image handling.
- Validated the Men's product inventory count and cart-counter behavior.
- Added negative login validation scenarios.
- Pushed selected Test Management cases into Low Code Automation.
- Used the Low-Code Authoring Agent to scaffold executable automation from natural-language test steps.
- Executed the resulting workflows in the BrowserStack cloud and produced a successful public build as submission evidence.
- Exported the refined manual test suite as CSV for the mission submission.

**What this demonstrates:** requirements analysis, AI-assisted test design, manual-to-automation workflow design, coverage refinement, and cloud execution.

---

## Mission 02 — Mastering Data & Enterprise Workflows
### Reusable Modules, Global Variables, and Secrets

**Goal:** Build maintainable end-to-end automation without hardcoded credentials or duplicated login/logout steps.

### What I Completed

- Built complete login → meaningful action → logout automated journeys in BrowserStack Low Code Automation.
- Created the reusable global variable **`UserEmail`** and used it across more than one automated workflow.
- Stored the password as the encrypted secret **`LoginPassword`**, keeping credentials out of plaintext test steps and execution logs.
- Refactored repeated authentication steps into reusable **Login** and **Logout** modules.
- Imported the reusable modules into a second test so only the unique middle workflow had to be created again.
- Verified the Global Variables **USED IN** count showed reuse across multiple tests.
- Executed both tests successfully in the BrowserStack cloud after correcting the configuration.
- Produced a passing public build with the reusable modules visible in the execution timeline.

**What this demonstrates:** maintainable automation architecture, secure test-data management, reuse, modular test design, and enterprise-style QA workflow practices.

---

## Mission 04 — The Resilient Pipeline
### AI Self-Healing Automation

**Goal:** Demonstrate that an automated test can recover from a changed UI locator without re-recording or manually editing the test.

### What I Completed

- Created a functional login automation and established a passing baseline.
- Used the Fashion Stack login page's **Toggle Button** to intentionally change element attributes and break the locator used by the test.
- Re-ran the unchanged automation with self-healing disabled and confirmed the locator failure.
- Enabled BrowserStack AI Self-Healing without re-recording or rewriting the test.
- Re-ran the exact same test and allowed BrowserStack to identify a replacement locator automatically.
- Verified the healed locator in the execution log and confirmed the **Self-Healed** badge appeared in the session history.
- Submitted a public session demonstrating the active self-healing result.

**What this demonstrates:** automation resilience, locator debugging, failure reproduction, AI-assisted maintenance, and the ability to validate recovery behavior rather than simply obtaining a passing result.

---

## Mission 05 — Test Case Mapping and Results Sync
### Automation-to-TCM Traceability

**Goal:** Connect automated Low Code Automation execution back to Test Management so automated results update the correct manual test cases.

### What I Completed

- Worked with an existing BrowserStack Test Management project and functioning Low Code Automation tests.
- Mapped automated tests to the appropriate Test Management test case IDs.
- Executed the mapped tests and exported XML test reports from the BrowserStack build.
- Produced multi-testcase XML reporting that included **TC-300** and **TC-301**.
- Uploaded the automated test results back into BrowserStack Test Management.
- Verified execution status updated against the mapped test cases rather than creating duplicate test cases.
- Captured Test Management results evidence showing successful traceability between automated execution and managed test cases.

**What this demonstrates:** requirements-to-execution traceability, test result synchronization, XML reporting, test management integration, and audit-friendly QA documentation.

---

## Project Outcome

This project went beyond running four isolated tests. It demonstrated an end-to-end QA workflow:

**User stories → AI-assisted test design → manual test refinement → low-code automation → reusable architecture → secure data handling → resilient execution → automated result synchronization.**

The final submission earned **2nd Place in the E-Commerce Track**. BrowserStack's evaluation team highlighted the submission's documentation quality, TC-300/TC-301 XML reports, and verified public Low Code Automation builds.

## Tools & Technologies

**BrowserStack:** Test Management, Low Code Automation, AI Test Case Generator, Low-Code Authoring Agent, AI Self-Healing, Global Variables, Secrets, Modules, cloud builds  
**Testing:** Functional Testing, Regression Thinking, Negative Testing, Edge-Case Testing, End-to-End Testing, Requirements Analysis, Test Case Design  
**Artifacts:** CSV Test Suite Export, XML Test Reports, Test Management Results, Public LCA Builds/Sessions

## Portfolio Summary

> Built and executed a four-mission BrowserStack AI Hackathon QA project for the Fashion Stack e-commerce application, combining AI-assisted test design, BrowserStack Test Management, Low Code Automation, reusable modules, secure variables/secrets, AI self-healing, and XML-based result synchronization. Designed coverage for carousel stability, product inventory, cart-counter behavior, and authentication edge cases. Earned 2nd Place in the E-Commerce Track, with BrowserStack recognizing the project as the cleanest four-mission submission in the competition.

## Project Links

- **Fashion Stack Demo:** https://ecommercebs.vercel.app/
- **GitHub Profile:** https://github.com/Ashl3yyMari3
- **LinkedIn:** https://linkedin.com/in/ashl3yymari3

### Evidence Note

The original BrowserStack submission included verified public LCA build/session links and exported XML reports. The exact public build URLs are not reproduced here because they were not available in the retained project materials used to assemble this portfolio page.
