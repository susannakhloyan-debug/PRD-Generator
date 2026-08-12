# PRD Generator

A BABOK v3–aligned Product Requirements Document generator for banking features.

Runs entirely client-side, no build step or server required.

## Usage

Open `index.html` in a browser (double-click it, or host it as a static page e.g. via GitHub Pages). Fill in the form — only **Product**, **Feature**, and **Author** are required — and click **Generate PRD** to produce a structured document. Any section left empty falls back to a sensible banking-domain default.

Covers: business need, objectives & KPIs, stakeholder RACI, elicitation summary, scope, current/future state, assumptions/constraints/dependencies, regulatory & compliance requirements (KYC, AML, PCI DSS, PSD2, GDPR, Basel III, SOX), business rules, epics & user stories with acceptance criteria, non-functional requirements, data requirements, risk assessment, sign-off, glossary, a traceability matrix, and a BABOK coverage checklist — the last two generated automatically from the rest.
