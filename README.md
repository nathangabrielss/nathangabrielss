<h1 align="center">Nathan Gabriel</h1>

<p align="center">
  <b>Data &amp; Analytics Engineer</b> · Supply Chain BI at <b>Minerva S.A</b><br>
  I build the full path from raw data to the screen where a decision gets made.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/nathangbrl"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:nathangabrielss@outlook.com"><img src="https://img.shields.io/badge/Email-333333?style=flat-square&logo=maildotru&logoColor=white" alt="Email"></a>
  <img src="https://img.shields.io/badge/Location-Brazil-009B3A?style=flat-square" alt="Brazil">
  <img src="https://komarev.com/ghpvc/?username=nathangabrielss&style=flat-square&color=333333&label=Profile+views" alt="Profile views">
</p>

---

## About

I work at the intersection of **data engineering, BI and application development** for supply chain.

Most of what I ship follows the same arc: model the data in the warehouse, publish it through a
governed semantic layer, then wrap it in a web application with authentication, permissions and
an audit trail — so the analysis is not just correct, but usable and accountable.

- Analytical SQL and dimensional modeling over layered (raw → refined → mart) warehouses
- Power BI semantic models, DAX and dataset governance
- Internal web platforms in Flask + TypeScript/React, with RBAC, JWT auth and audit logging
- Python data pipelines: ingestion, web scraping, Parquet publishing, scheduling and backups
- Documentation-as-code: every project I own has a versioned knowledge base next to the source

---

## Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white)

**Data &amp; BI**

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoftsqlserver&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black)
![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Apache Parquet](https://img.shields.io/badge/Parquet-50ABF1?style=flat-square&logo=apacheparquet&logoColor=white)
![SAP](https://img.shields.io/badge/SAP_data-0FAAFF?style=flat-square&logo=sap&logoColor=white)

**Backend &amp; Frontend**

![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white)
![REST](https://img.shields.io/badge/REST_APIs-02569B?style=flat-square)
![Pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

**Tooling**

![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![Obsidian](https://img.shields.io/badge/Obsidian-7C3AED?style=flat-square&logo=obsidian&logoColor=white)
![Claude](https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=anthropic&logoColor=white)
![Cursor](https://img.shields.io/badge/Cursor-000000?style=flat-square&logo=cursor&logoColor=white)

---

## What I actually do

| Area | What that means in practice |
|---|---|
| **Data modeling** | Fact and dimension design, slowly changing dimensions, reconciliation of ERP movements, stored procedures over layered warehouse schemas |
| **Semantic layer** | Power BI models, DAX measures, relationship design, contract-based datasets so downstream panels can't silently break |
| **Data pipelines** | Python ingestion from APIs, HTML, PDF and legacy spreadsheets; normalization; Parquet publishing; scheduled jobs with retry and outbox patterns |
| **Applications** | Flask backends and TypeScript/React frontends for internal operational systems — approvals, simulators, request desks, project books |
| **Security &amp; governance** | Role-based access control, JWT with refresh rotation, CSRF, rate limiting, irreversible hashing of personal identifiers, immutable audit logs, database segregation per domain |
| **Quality** | Automated test suites on business rules and access boundaries, backup routines with auditable records, design-system checklists before any visual change |
| **Documentation** | Every project carries its own "brain": architecture, modules, data sources, runbooks, decisions, backlog and risks — written alongside the code, not after it |

---

## Selected work

**Internal Supply Chain Portal** — Minerva S.A
A Flask portal that unifies authentication, authorization and navigation for the supply chain area,
hosting a set of independent operational and analytical modules behind a single sign-on shell.
Each module has its own database, its own declared roles and its own test-enforced boundary, so a
fault in an analytical module cannot reach the identity layer.
`Flask` `SQLite` `TypeScript` `React` `JWT` `pytest`

**Purchase Movement Data Model** — Minerva S.A
Analytical SQL over a layered warehouse, consolidating ERP purchase movements into fact tables
used by the area's corporate reporting. Includes dimension corrections, historical reconciliation
and regression tests against known reference periods.
`SQL` `Dimensional modeling` `ERP data`

**Economic Scenario Pipeline**
A Python pipeline with dozens of connectors that collects macroeconomic and commodity indicators
from statistics institutes, central bank PDFs, legacy spreadsheets and market quotes, normalizes
them into a single series format and publishes them to an internal panel.
`Python` `BeautifulSoup` `pandas` `Parquet`

**Purchasing Indicators Panel**
A read-only analytical runtime that reads YAML contracts and queries published Parquet through
DuckDB, keeping the panel decoupled from the warehouse while guaranteeing that filters and
definitions match the governed dataset.
`DuckDB` `YAML contracts` `Parquet`

> Most of my day-to-day work lives in private, corporate repositories. The public repositories here
> are studies, experiments and personal projects.

---

## GitHub

<p align="center">
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=nathangabrielss&theme=github_dark" alt="Profile details">
</p>

<p align="center">
  <img height="190" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=nathangabrielss&theme=github_dark" alt="Most used languages">
  <img height="190" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=nathangabrielss&theme=github_dark" alt="Stats">
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=nathangabrielss&hide_border=true&theme=github-dark" alt="Contribution streak">
</p>

---

## How I work

- **Impact, risk, validation.** Every technical decision gets justified on those three axes before it ships.
- **Nothing destructive without explicit approval.** Databases, branches and semantic models are changed with the current state, the proposal and the expected impact on the table first.
- **Validate in the real environment.** Documentation is a map, not the territory — code, database and terminal win when they disagree.
- **Documentation is born with the project**, not bolted on at the end.

---

## Currently

- Deepening **NoSQL databases** and **applied programming** through my degree
- Expanding the portal's module catalog and tightening its automated test coverage
- Studying agent-assisted engineering workflows and how to govern them inside a corporate environment

---

<p align="center">
  <i>Open to conversations about data engineering, BI architecture and internal platform development.</i>
</p>
