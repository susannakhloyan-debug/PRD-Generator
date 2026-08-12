# PRD Generator

A BABOK v3–aligned Product Requirements Document generator for banking features.

Runs entirely client-side, no build step or server required.

## Usage

### Open it

- **Live demo:** https://susannakhloyan-debug.github.io/PRD-Generator/
- **Locally:** double-click `index.html`, or drag it into a browser tab — no install, no build step.
- **Self-hosted:** copy `index.html` to any static host (GitHub Pages, S3, an internal file share) and open it there.

### Fill in the form

The left-hand rail lets you jump straight to any section. Only three fields are required to generate a document:

| Field | Where |
|---|---|
| Product / system name | "Product, feature & author" |
| Feature / epic | "Product, feature & author" |
| Author (you) | "Product, feature & author" |

Everything else is optional — business unit, version, status, priority, target release, and classification live under the collapsible "Document details" within that same section. Below it, work through as many of the numbered sections as you have information for: business need, objectives & KPIs, stakeholders (RACI), elicitation summary, scope, current/future state, assumptions/constraints/dependencies, regulatory & compliance requirements, business rules, epics & user stories (with Given/When/Then acceptance criteria), non-functional requirements, data requirements, risks, sign-off approvers, and a glossary. Repeatable fields (objectives, stakeholders, risks, etc.) have their own **+ Add** button; epics have **+ Add user story**, and each story has **+ Add acceptance criterion**.

You don't have to fill in every section — anything left blank is replaced with a sensible banking-domain default when the document is generated, so a minimal PRD (just Product/Feature/Author) is still a complete, coherent document.

Two shortcuts at the top of the page help you get oriented:

- **Load an example** — fills the entire form with a worked example ("Instant Card Freeze & Unfreeze") so you can see what a complete PRD looks like before writing your own.
- **Clear all fields** — resets the form back to empty.

### Generate the document

Click **Generate PRD** (top right, always visible). If Product, Feature, or Author is missing, the page scrolls to and highlights the first missing field instead of generating. Once all three are present, a `.docx` file downloads automatically, named after your feature (e.g. `Instant_Card_Freeze_Unfreeze_PRD.docx`), and a banner appears with a link to download it again without regenerating.

Covers: business need, objectives & KPIs, stakeholder RACI, elicitation summary, scope, current/future state, assumptions/constraints/dependencies, regulatory & compliance requirements (KYC, AML, PCI DSS, PSD2, GDPR, Basel III, SOX), business rules, epics & user stories with acceptance criteria, non-functional requirements, data requirements, risk assessment, sign-off, glossary, a traceability matrix, and a BABOK coverage checklist — the last two generated automatically from the rest.
