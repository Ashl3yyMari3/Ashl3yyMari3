# Mission 04: The Resilient Pipeline

## Goal

Prove that BrowserStack AI Self-Healing can recover an automated test after a UI locator changes, without re-recording or manually rewriting the test.

## Requirements

BrowserStack required participants to:

1. Create a functional login automation and get a passing baseline.
2. Use the FashionStack Toggle Button to change the target element attributes and break the locator.
3. Rerun the unchanged test and confirm the altered element causes the test to fail.
4. Enable **Self-Healing** and rerun the exact same test.
5. Open the execution log and verify the healed locator and **Self-Healed** indicator.

## Required submission evidence

- Public session URL displaying the active **Self-Healed** indicator in the Low Code Automation execution-log history.

## What I built

A three-stage BrowserStack Low Code Automation sequence using the test `M04 - AI Self healing Login`:

1. Passing baseline
2. Intentional locator failure
3. Passing rerun after the self-healing stage

## Build evidence

| Build | Time | Result | Purpose |
| --- | --- | --- | --- |
| `M4 AI Self Healing-1` | Aug 13, 2026, 12:26:55 AM EDT | Passed | Baseline working automation |
| `M4 AI Self Healing-2` | Aug 13, 2026, 12:43:47 AM EDT | Failed | Intentional locator failure |
| `M4 AI Self Healing-3` | Aug 13, 2026, 12:46:18 AM EDT | Passed | Subsequent successful rerun |

The failed execution identifies the step:

`Hover over "Back to Home" button`

and records the BrowserStack error:

`Could not find element on the page. Please file a bug or re-record the test step.`

### Detailed run history

[`run-history.md`](./run-history.md)

## Evidence note

The original hackathon submission included the required public self-healing session. The current BrowserStack account view still exposes the historical builds and execution steps, but the original public session token / visible historical Self-Healed badge is no longer available through the current access level. This folder preserves the recovered **pass -> locator failure -> subsequent pass** history without inventing a replacement public link.

## Skills demonstrated

Failure reproduction, locator debugging, automation resilience, AI-assisted test maintenance, root-cause investigation, and validation of recovery behavior.
