# PRD Generator

A BABOK v3–aligned Product Requirements Document generator for banking features.

Runs entirely client-side, no build step or server required.

## Usage

Open `index.html` in a browser (double-click it, or host it as a static page e.g. via GitHub Pages). Fill in the form — only **Product**, **Feature**, and **Author** are required — and click **Generate PRD** to produce a structured document. Any section left empty falls back to a sensible banking-domain default.

Covers: business need, objectives & KPIs, stakeholder RACI, elicitation summary, scope, current/future state, assumptions/constraints/dependencies, regulatory & compliance requirements (KYC, AML, PCI DSS, PSD2, GDPR, Basel III, SOX), business rules, epics & user stories with acceptance criteria, non-functional requirements, data requirements, risk assessment, sign-off, glossary, a traceability matrix, and a BABOK coverage checklist — the last two generated automatically from the rest.

## Draft with AI (optional)

The **Draft with AI** panel at the top of the form uses Claude to turn rough notes (a meeting summary, a one-line feature idea) into a first-pass draft, then runs a second pass that reviews its own draft against INVEST and testability before applying it to the form.

- Requires an [Anthropic API key](https://platform.claude.com/settings/keys), pasted into the panel. The key is stored only in your browser's `localStorage` and is sent directly from your browser to `api.anthropic.com` — there is no server in this project to route it through.
- It never overwrites a field you've already filled in — only empty fields and empty sections get populated, so you can fill in what you know and let AI fill the rest, in either order.
- Anything the model had to guess at is surfaced as an **open question** in the status area instead of being silently invented — resolve those before you generate the final document.
- This mode calls the Anthropic API directly from the page (`anthropic-dangerous-direct-browser-access`) and bills to your own API key at standard Claude API rates.

Everything else about the tool — the static form, the manual generation flow, the download — works exactly as before and requires no API key.
