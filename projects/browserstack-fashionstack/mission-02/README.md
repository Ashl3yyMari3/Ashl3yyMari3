# Mission 02: Mastering Data & Enterprise Workflows

## Goal

Build a complete **login -> action -> logout** journey, then refactor it into a maintainable enterprise-style automation design using shared variables, encrypted credentials, and reusable modules.

## Requirements

BrowserStack required participants to:

1. Create a Global Variable such as `UserEmail`.
2. Create an encrypted Secret such as `LoginPassword`.
3. Record a complete login, meaningful in-app action, and logout workflow.
4. Replace hardcoded email/password values with the Global Variable and Secret.
5. Confirm no plaintext credentials remained in the test steps.
6. Turn repeated login steps into a reusable `Login` module.
7. Turn repeated logout steps into a reusable `Logout` module.
8. Create a second test with a different middle action while reusing the same Login and Logout modules.
9. Confirm `UserEmail` showed a **USED IN** count greater than one.
10. Execute both tests successfully in the BrowserStack cloud.

## Required submission evidence

- Public build link showing **both tests passing**, with the Login and Logout modules visible in the execution timeline.
- Screenshot of the Global Variables page showing the shared variable used across multiple tests.

## What I built

- `M02 - Login, Add to Cart, and Logout`
- `M02 - Login, Verify Men Inventory, and Logout`
- Shared `UserEmail` Global Variable
- Encrypted `LoginPassword` Secret
- Reusable `Login` and `Logout` modules
- Two successful end-to-end cloud workflows

## Build evidence

### Public BrowserStack build

https://low-code.browserstack.com/projects/4020759/builds/ytmqporhxmztcmrvt85rxaeovoo9graunciiswff?public_token=050912ea5a7e3216116e481201f3f9d621b193b7288696c8ae5ae8bf7b1c782f

**Build:** `M02 - FashionStack Enterprise Workflows-6`  
**Result:** Passed  
**Tests:** 2 passed, 0 failed

- `M02 - Login, Add to Cart, and Logout` — Passed
- `M02 - Login, Verify Men Inventory, and Logout` — Passed

## Evidence recovered

The public build remains accessible and verifies both Mission 02 workflows passed. The original BrowserStack project also showed the shared-variable/module configuration used to make the workflows reusable rather than duplicating authentication steps.

## Skills demonstrated

Reusable automation architecture, secure test-data handling, encrypted secrets, global variables, modular workflow design, end-to-end testing, and maintainable enterprise QA practices.
