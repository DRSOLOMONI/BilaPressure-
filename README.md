# Bila Pressure 🇰🇪

**Your life. Your pace. Your choice.**

Bila Pressure is an early-stage, privacy-conscious project exploring supportive habit reflection, responsible data insights, and future community resources for adults aged **18–29 in Kenya**.

> **Status:** Interactive front-end prototype. This is not a medical product, has no real AI integration, and has not been evaluated for effectiveness.

## Try the prototype

Open **[index.html](./index.html)** in a browser, or enable GitHub Pages to host the static prototype. The current version offers:
- Optional daily mood and intention check-in.
- Optional reflection on influences and a private note.
- A recent-entry view and simple personal snapshot.
- Export and delete controls.
- Safety and privacy notices.

**Privacy note:** Entries are stored in browser-local storage on the device. There is no backend, account system, shared database, or network upload of check-in entries in this prototype. Anyone with access to the same browser profile may be able to see them. Exported files may also contain sensitive information.

## One platform, three connected components

1. **Bila Pressure Coach** — the core experience: private check-ins, personal intentions, and non-judgmental reflection.
2. **Bila Pressure Insights** — a data portfolio using synthetic data, Excel, SQL, Python, and Power BI to explore usability and engagement responsibly.
3. **Bila Pressure Community** — a possible later stage for educational resources and supportive challenges, only after demand, safeguarding, moderation, and privacy requirements are validated.

Only the first component has a basic front-end prototype today. The analytics workflow and community are planned—not built.

## Repository guide

- `index.html` — static interactive prototype.
- `docs/problem_statement.md` — research questions, assumptions, scope, and safeguards.
- `docs/roadmap.md` — phased plan and decision gates.
- `docs/data_dictionary.md` — prototype fields, storage behavior, and future synthetic-data rules.

## Development principles

- Adults 18+ only.
- Treat assumptions as questions to test, not established facts.
- Use synthetic data for public demos and portfolio analysis.
- Collect the minimum necessary data and explain its purpose.
- No diagnosis, treatment claims, or unsupported promises of effectiveness.
- Seek qualified health-professional input before adding health-related guidance.
- People who may be physically dependent on alcohol should consult a qualified healthcare professional before suddenly stopping; withdrawal can be dangerous.
- Evaluate usability, safety, and outcomes separately. Engagement alone does not demonstrate reduced alcohol-related harm.

## Roadmap

1. Define and validate the problem.
2. Test prototype usability with appropriate safeguards.
3. Build a documented synthetic dataset and reproducible cleaning workflow.
4. Analyze the data with SQL/Python and build a Power BI dashboard.
5. Review safety, privacy, accessibility, and product requirements.
6. Consider a controlled pilot only with an appropriate protocol and consent.
7. Make no effectiveness claims without suitable evidence.

## Technology

- HTML, CSS, JavaScript for the initial static prototype.
- Planned portfolio tools: Excel, SQL, Python, Power BI.
- Next.js/React, backend services, and AI are future options—not current capabilities.

## Project status and contribution

This project is being developed iteratively. Start with the problem statement and roadmap before expanding features. Do not commit personal, identifiable, or sensitive health data to this public repository.

Bila Pressure is an independent learning project, not a substitute for professional healthcare.
