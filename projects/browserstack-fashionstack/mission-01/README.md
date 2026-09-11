# Mission 01: The AI Test Architect

## Goal

Generate a complete manual test suite from the supplied FashionStack user stories, refine the AI-generated coverage, push selected cases into BrowserStack Low Code Automation, and execute the generated workflow in the cloud.

## Requirements

BrowserStack required participants to:

1. Create a Test Management project for the FashionStack application.
2. Use the AI Test Case Generator to generate cases for the supplied user stories.
3. Review and refine the suite so it included core paths, negative validation flows, and edge cases.
4. Select at least two manual test cases and push them into Low Code Automation.
5. Use the Low-Code Authoring Agent to scaffold executable automation from the natural-language test steps.
6. Execute the workflow on BrowserStack cloud browser configurations.

### User stories covered

- **US-01: Homepage Hero Carousel** — dynamic carousel content, navigation, rapid interaction stability, and broken/missing content handling.
- **US-02: Men's Category Inventory** — Men's Fashion page, expected **16 products**, product-card content, images, and detail navigation.
- **US-03: Persistent Cart Counter** — Add to Cart behavior, counter updates, persistence across navigation, quantity/repeated-add behavior, and missing-size validation.
- **US-04: Authentication** — successful login/logout, invalid credentials, invalid/blank input, password masking, and authentication-state behavior.

## Required submission evidence

- Exported CSV of the refined manual test suite from Test Management.
- Public build link showing successful execution of the generated Low Code Automation script.

## What I built

- A **16-case FashionStack manual test suite**, with four test cases for each user story.
- Happy Path, Negative, and Edge Case coverage.
- Structured case IDs, priorities, scenario classifications, detailed descriptions, and direct BrowserStack Test Management links.
- Selected Test Management cases used later for automation and result mapping, including **TC-300** and **TC-301**.

## Evidence

### Full 16-case spreadsheet

[`M01_FashionStack_Manual_Test_Suite_16_Cases.csv`](./M01_FashionStack_Manual_Test_Suite_16_Cases.csv)

The spreadsheet contains all 16 FashionStack cases and preserves the BrowserStack Test Management case IDs and direct case URLs.

## Build evidence

The Mission 01 submission originally required a successful public Low Code Automation build. The retained portfolio materials currently preserve the full manual Test Management suite, but the original Mission 01 public build URL has not been recovered. No replacement link is being fabricated.

## Skills demonstrated

Requirements analysis, AI-assisted test generation, manual test refinement, positive/negative/edge-case test design, Test Management, manual-to-automation workflow design, and cloud execution.
