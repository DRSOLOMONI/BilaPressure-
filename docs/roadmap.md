# Bila Pressure Roadmap

This roadmap deliberately keeps the first release small. Each phase should produce evidence before the next phase expands scope.

## Phase 1 — Problem discovery
- [ ] Review `docs/problem_statement.md`.
- [ ] Draft a short, voluntary research guide for adults 18+.
- [ ] Validate the guide with a qualified health professional or appropriate research adviser.
- [ ] Record themes without names or identifying details.
- [ ] Decide whether the problem and proposed audience are sufficiently supported.

**Gate:** Do not collect sensitive personal or health data without appropriate consent and safeguards.

## Phase 2 — Prototype usability
- [x] Create a responsive, browser-based check-in prototype.
- [x] Add personal intention, mood, optional reflection, recent entries, export, and delete.
- [x] Keep data in browser-local storage; no server upload.
- [x] Label inactive AI and community features honestly.
- [ ] Test on mobile and desktop; check accessibility and browser storage behavior.
- [ ] Gather voluntary usability feedback from adults, without treating feedback as evidence of health impact.

**Gate:** Fix confusing language, accessibility problems, and privacy risks before any wider pilot.

## Phase 3 — Data foundation
- [ ] Create a documented synthetic dataset with no real participant records.
- [ ] Define field names, types, allowed values, missing-value rules, and limitations.
- [ ] Clean and validate in Python or Excel.
- [ ] Load the synthetic data into a relational model and practice SQL analysis.
- [ ] Document every transformation and create reproducible scripts.

## Phase 4 — Power BI insights
- [ ] Define product metrics such as check-in completion and return usage.
- [ ] Build a dashboard from synthetic data.
- [ ] Show denominators, time windows, missing data, and limitations.
- [ ] Avoid presenting engagement metrics as proof of reduced alcohol-related harm.

## Phase 5 — Safety and product decision
- [ ] Obtain qualified health-professional input before adding health-related guidance.
- [ ] Define safe responses for distress, dependence concerns, and requests for diagnosis.
- [ ] Assess data protection, consent, retention, deletion, and security needs.
- [ ] Decide whether a real AI feature is necessary. If used, evaluate it with safety tests and clear limitations.
- [ ] Design community features only after trust, moderation, reporting, and safeguarding requirements are understood.

## Phase 6 — Controlled pilot and evaluation
- [ ] Set a written protocol and appropriate approvals before recruiting participants.
- [ ] Establish baseline, outcome definition, follow-up window, and missing-data plan.
- [ ] Use consented data and minimize collection.
- [ ] Evaluate feasibility and safety first; do not imply causal effectiveness without a suitable design.
- [ ] Publish limitations and negative or inconclusive findings honestly.

## Phase 7 — Launch readiness
- [ ] Complete security, accessibility, and privacy review.
- [ ] Prepare support signposting and incident-handling process.
- [ ] Review legal and data-protection obligations for the intended jurisdiction.
- [ ] Test backups, deletion, and recovery if any server-side storage is introduced.
- [ ] Launch only after safety, research, and operational gates are met.

## Current technical state

The initial `index.html` is a static front-end prototype. It does **not** contain a backend, account system, real AI integration, or shared database. Local entries are stored in the browser on the device. GitHub Pages can host the static interface, but hosting the page does not send browser-local entries to the repository.
