# IT Controls Assurance Toolkit — Demonstration

A self-contained, single-page demonstration of an **open-source-style toolkit
of reusable scripts and templates for IT audit & GRC**, organized into cohesive
**modules** and framed as *compliance as code*:

- **Toolkit modules** — a filterable, expandable grid of 7 modules across the
  assurance lifecycle: **ITGC Evidence Collector**, **Access Recertification &
  SoD Analyzer**, **Control Test Runner**, **Policy/Report Generator (Jinja2)**,
  **Framework Crosswalk Builder**, **Multi-Cloud Compliance Guardrails**, and a
  **CI Policy-as-Code Gate** — each with inputs/outputs and a numbered run
  sequence.
- **Automation code** — accurate, well-commented examples in **Python** (control
  test runner → JSON + JUnit, and a Jinja2 report generator), **Bash** (ITGC
  evidence collector), **PowerShell** (AD/Entra access review + SoD), **SQL**
  (audit sampling, recertification exceptions, terminated-still-active),
  **Ansible** (CIS-style baseline play), **GitHub Actions** (CI gate), and
  **OPA/Rego** (Conftest policy).
- **Multi-cloud guardrails** — the same control intent as IaC across **AWS**
  (CloudFormation Config rules + SCPs), **Azure** (Bicep Azure Policy), and
  **GCP** (Organization Policy constraints).
- **Framework mapping**, an **architecture + CI pipeline** diagram, and
  **spreadsheet artifacts** (a Risk-Control Matrix and audit checklist as CSV).

Control references map to **NIST SP 800-53**, the **CIS Critical Security
Controls**, **ISO/IEC 27001:2022**, and the **AICPA SOC 2 Trust Services
Criteria**.

## 🔗 Live demo

**https://smittystuff.github.io/ita-grc-toolkit/**

## About

The toolkit, scripts, evidence, and organization are **illustrative and
fictional** — a simplified sample included only to demonstrate methodology,
engineering approach, and deliverables. Validate all mappings and code against
current standards and your own environment before relying on them.

## Tech

A single `index.html` — no build step, no dependencies. All styling and
interactivity (module filter, expandable module rows, code tabs, cloud
guardrail tabs) are inline vanilla HTML/CSS/JS, so it deploys anywhere static
files are served. The illustrative toolkit itself spans Python, Bash,
PowerShell, SQL, Ansible, GitHub Actions, Jinja2, OPA/Conftest, and multi-cloud
IaC (CloudFormation, Bicep, GCP Org Policy).

## Run locally

```bash
python3 -m http.server 8080
# then visit http://localhost:8080
```

---

Part of the portfolio of Steven Smith — Information Security Consultant.
