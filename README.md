# Automated Commerce Identity Room

## One-sentence benefit

Verify which organisation an automated trading system represents and what it is authorised to do.

## Live demo

[Watch the workflow](docs/demo.webm).

## Screenshots

![Automated commerce identity dashboard](docs/screenshot.png)

## Main features

- Search and sort identity cases by system, business, credential or status.
- Create real identity cases through the Java API.
- Advance cases through draft, review and approved states.
- Show loading, empty, error and success feedback.
- Present operational and guidance sections responsively.

## Technology used

Angular, TypeScript, signals, HttpClient, SSR, Spring Boot and Java 21.

## Installation instructions

Install Node.js 22 and Java 21. Run `npm install`, start `cd backend && mvn spring-boot:run`, then run `npm start`.

## Commercial licensing/contact

Commercial licensing and integration support are available through the repository contact options.

## Business problem and users

Businesses and counterparties need trusted proof of the organisation, delegation and transaction scope behind automated systems.

## Key workflows

Find an automated system, add an identity case, review delegated powers, advance approval and confirm the API result.

## Angular framework highlights

Signals provide derived state, OnPush change detection limits work, HttpClient performs real API writes and SSR remains configured.

## Java backend highlights

Spring Boot exposes validated list, search, create and update APIs, clear errors, health status and service tests.

## Architecture and state flow

Angular calls `/api/items`; Java validates requests and returns updated identity cases to signal-based state.

## Accessibility and responsive behaviour

Semantic sections, labelled search, visible focus styles and responsive work rows support keyboard and small screens.

## Verification commands

Run `npm test`, `npm run build`, `cd backend && mvn test` and `cd backend && mvn package`.

## Structure

`src` contains the frontend, `backend` contains Java and `docs` contains inspected media.

## Tradeoffs

In-memory records simplify local use; production needs wallet verification, persistence and trading-platform integrations.

## Roadmap

Add credential proofs, delegation expiry, transaction limits, counterparty receipts and multilingual trust notices.
