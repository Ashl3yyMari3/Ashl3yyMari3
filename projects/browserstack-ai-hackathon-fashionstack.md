# BrowserStack AI Hackathon: Fashion Stack E-Commerce QA Project

## Ashley Cichy | QA Engineer & Computer Science Student

**Achievement:** 2nd Place Winner, E-Commerce Track  
**Demo Application:** https://ecommercebs.vercel.app/  
**Platform:** BrowserStack Test Management + Low Code Automation  
**Evidence Archive:** [Recovered mission artifacts and build evidence](./browserstack-fashionstack/evidence/README.md)

## Project Overview

I completed four qualifying technical missions for BrowserStack's Fashion Stack e-commerce challenge: **Mission 01, Mission 02, Mission 04, and Mission 05**.

The challenge allowed participants to complete any four of six technical missions. My submission demonstrated an end-to-end QA workflow that moved from raw product requirements into AI-assisted test design, manual test refinement, low-code automation, reusable architecture, secure test data, locator-failure recovery, and synchronized Test Management results.

BrowserStack's evaluation team recognized the project as the **cleanest four-mission submission in the competition**, specifically praising the documentation, the multi-testcase XML reports for **TC-300** and **TC-301**, and verified Low Code Automation public build links.

### End-to-End QA Flow

**User stories -> AI-assisted test design -> manual test refinement -> Low Code Automation -> reusable modules and secure test data -> self-healing workflow -> Test Management result synchronization**

### Core Skills Demonstrated

- Requirements analysis and test case design
- Positive, negative, boundary, and edge-case coverage
- BrowserStack Test Management
- BrowserStack Low Code Automation
- AI Test Case Generator and Low-Code Authoring Agent
- Reusable Login and Logout modules
- Global variables and encrypted secrets
- Cloud-based automated execution
- AI-assisted locator recovery / self-healing
- XML/JUnit result reporting
- Automation-to-Test Management traceability

---

# Mission 01: The AI Test Architect
## TCM and LCA Generation

### What the challenge required

Participants had to turn the supplied FashionStack user stories into a structured manual test suite and then convert selected cases into executable Low Code Automation workflows.

The required workflow was:

1. Create a BrowserStack Test Management project.
2. Use the AI Test Case Generator to generate cases from the supplied user stories.
3. Review and refine the generated suite so it included core paths, negative scenarios, and edge cases.
4. Select at least two manual test cases and push them into Low Code Automation.
5. Use the Low-Code Authoring Agent to scaffold automation from the natural-language steps.
6. Execute the workflow in the BrowserStack cloud.

### Required submission evidence

- Exported CSV of the refined manual test suite from Test Management
- Public build link showing successful execution of the generated Low Code Automation script

### FashionStack requirements covered

**US-01: Homepage Hero Carousel**
- Validate the dynamic hero carousel.
- Cover normal slide transitions and navigation.
- Verify interaction stability, including rapid navigation.
- Include missing/broken-content behavior.

**US-02: Men's Category Inventory**
- Clicking **Men** should open the page headed **Men's Fashion**.
- The inventory summary should contain **16 products**.
- Exactly 16 product cards should be displayed.
- Product cards should contain a product name, price, image/fallback, and working details navigation.

**US-03: Persistent Cart Counter**
- Start from a clean cart state.
- Add a product and verify the cart counter updates correctly.
- Verify the cart count persists across navigation.
- Include repeated-add, quantity-change, and missing-size scenarios.

**US-04: Authentication**
- Validate successful login and logout.
- Cover incorrect password, unregistered email, invalid email format, and blank fields.
- Verify password masking.
- Include OTP authentication where available.

### What I built

- Created the FashionStack Test Management project.
- Generated and refined test cases across all four user stories.
- Structured coverage across happy paths, negative tests, and edge cases.
- Pushed selected Test Management cases into Low Code Automation.
- Used the Low-Code Authoring Agent to create executable workflows.
- Executed the automation in BrowserStack's cloud environment.

### Recovered evidence

- [Mission 01 Test Management CSV export](./browserstack-fashionstack/evidence/mission-01-test-management-export.csv)
- The recovered CSV contains **TC-300**, detailed preconditions, atomic test steps, exact expected results, project metadata, and the AI refinement prompt documenting the full 16-case test structure across US-01 through US-04.

**What this demonstrates:** requirements analysis, AI-assisted test design, manual-to-automation workflow design, coverage refinement, and cloud execution.

---

# Mission 02: Mastering Data & Enterprise Workflows
## Reusable Modules, Global Variables, and Secrets

### What the challenge required

Participants had to build one complete **login -> action -> logout** journey and then refactor it into an enterprise-style reusable test design.

The workflow required:

1. Create a global variable such as `UserEmail`.
2. Store the password as an encrypted secret such as `LoginPassword`.
3. Build a complete login, meaningful in-app action, and logout workflow.
4. Replace hardcoded data with the global variable and encrypted secret.
5. Confirm no plaintext credential remained in the test steps.
6. Convert the repeated login steps into a reusable `Login` module.
7. Convert the repeated logout steps into a reusable `Logout` module.
8. Create a second test performing a different in-app action and import the same modules.
9. Verify the shared variable showed a USED IN count greater than one.
10. Run both tests successfully in BrowserStack's cloud.

### Required submission evidence

- Public build link showing both tests passing with the Login and Logout modules visible
- Screenshot of the Global Variables page showing the variable reused across multiple tests

### What I built

- `M02 - Login, Add to Cart, and Logout`
- `M02 - Login, Verify Men Inventory, and Logout`
- Shared `UserEmail` global variable
- Encrypted `LoginPassword` secret
- Reusable Login and Logout modules
- Two passing end-to-end cloud workflows

### Live evidence

**Public BrowserStack build:**  
https://low-code.browserstack.com/projects/4020759/builds/ytmqporhxmztcmrvt85rxaeovoo9graunciiswff?public_token=050912ea5a7e3216116e481201f3f9d621b193b7288696c8ae5ae8bf7b1c782f

**Recovered build:** `M02 - FashionStack Enterprise Workflows-6`  
**Result:** 2 tests passed, 0 failed

**What this demonstrates:** reusable automation architecture, secure test-data management, modular workflow design, and maintainable enterprise QA practices.

---

# Mission 04: The Resilient Pipeline
## AI Self-Healing Automation

### What the challenge required

This mission intentionally broke a working locator and required BrowserStack's self-healing capability to recover without re-recording the test.

The required sequence was:

1. Create a functional login automation and establish a passing baseline.
2. Use the FashionStack Toggle Button to change the target element attributes.
3. Rerun the unchanged test and confirm the altered locator causes a failure.
4. Enable Self-Healing and rerun the exact same test.
5. Verify the healed locator and Self-Healed indicator in the execution history.

### Required submission evidence

- Public session URL displaying the active **Self-Healed** indicator in the Low Code Automation execution history

### Recovered original run sequence

The historical BrowserStack project still preserves the mission's pass/fail/pass progression:

- **`M4 AI Self Healing-1`**: Passed, Aug 13, 2026 at 12:26:55 AM EDT
- **`M4 AI Self Healing-2`**: Failed, Aug 13, 2026 at 12:43:47 AM EDT
- **`M4 AI Self Healing-3`**: Passed, Aug 13, 2026 at 12:46:18 AM EDT

The failed execution shows the step:

`Hover over "Back to Home" button`

with the BrowserStack error:

`Could not find element on the page. Please file a bug or re-record the test step.`

That failure is the deliberate middle stage of the mission, followed minutes later by the passing M4-3 execution.

### Recovered evidence

- [Mission 04 recovered run history](./browserstack-fashionstack/evidence/mission-04-run-history.md)

**Evidence note:** The original competition submission included the required public self-healing session. The current account view still exposes the historical builds and execution steps, but the original public session token / visible historical Self-Healed badge is not currently available. The portfolio therefore preserves the recovered pass -> locator failure -> subsequent pass sequence without presenting an unverifiable current public badge link.

**What this demonstrates:** failure reproduction, locator debugging, resilient automation, AI-assisted maintenance, and validation of recovery behavior rather than simply chasing a green test result.

---

# Mission 05: Test Case Mapping and Results Sync
## Automation-to-TCM Traceability

### What the challenge required

Participants had to connect Low Code Automation execution back to BrowserStack Test Management so automated results landed against the correct managed test cases.

The required workflow was:

1. Start with an existing Test Management project and a working Low Code Automation test.
2. Map the automated test to Test Management case IDs.
3. Execute the mapped automation and download the XML report from the build.
4. Upload the result into Test Management and confirm execution status updates against the mapped cases.

### Required submission evidence

- Test Management test-run screenshot showing execution results
- Exported XML report

### What I built

- Mapped automated FashionStack tests to Test Management cases.
- Executed the mapped tests in Low Code Automation.
- Exported a multi-testcase XML report.
- Synchronized the automation results back into Test Management.
- Verified the results updated the mapped cases instead of creating duplicates.

### Recovered evidence

**Public BrowserStack M05 build:**  
https://low-code.browserstack.com/projects/4024697/builds/rfjctl2wtr2solhyvcnahd4jmvtbrnygswrahtuy?public_token=ab46fe7fc2f4b17a7941c190b95981701d8eb1784109c61ebf5651c17becea1b

**XML report:**  
[Mission 05 TCM Results XML](./browserstack-fashionstack/evidence/mission-05-tcm-results.xml)

The recovered XML records:

- Test suite: `M05 - TCM Results Sync-1`
- **2 tests**
- **0 failures**
- Chrome desktop execution
- **TC-300:** `M01-US02: Clicking Men Opens Men's Fashion Page with Exactly 16 Product Listings`
- **TC-301:** `M01-US02: Product Names, Prices, and Images Display Correctly and Navigate to Detail Pages`

The recovered Test Management run shows:

- `M05 - FashionStack LCA Results Sync #1`
- Created by Ashley Cichy on Aug 13, 2026
- 2 tests
- 2m 49s duration
- **2 passed, 0 failed**
- Failure analysis: **No Failures**

The recovered Project Insights view also shows:

- **16 total test cases**
- **14 manual test cases**
- **2 automated test cases**
- **12.50% automation coverage**

**What this demonstrates:** requirements-to-execution traceability, XML/JUnit reporting, results synchronization, Test Management integration, and audit-friendly QA documentation.

---

# Evidence Archive

The preserved evidence is organized here:

**[Open the FashionStack Evidence Index](./browserstack-fashionstack/evidence/README.md)**

Current archive includes:

- Mission 01 Test Management CSV export
- Mission 02 public passing BrowserStack build
- Mission 04 recovered build/run history
- Mission 05 public BrowserStack build
- Mission 05 XML report with TC-300 and TC-301
- Recovered Test Management execution details and project metrics

---

# Project Outcome

This project was more than a collection of isolated tests. It demonstrated a complete QA lifecycle across requirements, test management, automation design, execution resilience, and reporting.

The final submission earned **2nd Place in the BrowserStack AI Hackathon E-Commerce Track**. BrowserStack specifically recognized the quality of the documentation, the multi-testcase TC-300 / TC-301 XML reporting, and verified Low Code Automation build evidence.

## Tools & Technologies

**BrowserStack:** Test Management, Low Code Automation, AI Test Case Generator, Low-Code Authoring Agent, AI Self-Healing, Global Variables, Secrets, Modules, cloud builds  
**Testing:** Functional Testing, Negative Testing, Edge-Case Testing, End-to-End Testing, Requirements Analysis, Test Case Design, Traceability  
**Artifacts:** CSV Test Management Export, XML/JUnit Report, BrowserStack Build Results, Test Management Run Results

## Portfolio Summary

> Built and executed a four-mission BrowserStack AI Hackathon QA project for the Fashion Stack e-commerce application, combining AI-assisted test design, Test Management, Low Code Automation, reusable modules, secure variables and secrets, AI self-healing workflows, and XML-based result synchronization. Designed coverage for carousel stability, product inventory, persistent cart behavior, and authentication scenarios. Earned 2nd Place in the E-Commerce Track, with BrowserStack recognizing the project as the cleanest four-mission submission in the competition.

## Links

- **Fashion Stack Demo:** https://ecommercebs.vercel.app/
- **Evidence Archive:** [GitHub evidence folder](./browserstack-fashionstack/evidence/README.md)
- **GitHub Profile:** https://github.com/Ashl3yyMari3
- **LinkedIn:** https://linkedin.com/in/ashl3yymari3
