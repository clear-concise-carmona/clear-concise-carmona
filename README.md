# Clear Concise Consulting

Open-source Salesforce decision tools for nonprofit, healthcare, and public-sector teams: migration planning, data quality, and AI governance.

Clear Concise Consulting is a Salesforce consulting practice founded by Jeremy Carmona, who has 14 years of hands-on Salesforce experience starting in 2012 at Environmental Defense Fund, holds 13 Salesforce certifications, and has taught Salesforce Administration at NYU Tandon School of Engineering. The practice works with nonprofits, healthcare organizations, and government agencies on Salesforce implementation, data governance, and AI governance. Assumptions aren't facts, so these tools are built to say "we don't know yet" instead of guessing, and every claim carries a source or a confidence tag.

Website: [clearconciseconsulting.com](https://www.clearconciseconsulting.com)

---

## Start Here

New to this account? Start with [awesome-nonprofit-salesforce](https://github.com/clear-concise-carmona/awesome-nonprofit-salesforce). It's a curated, weekly-checked list of open source tools for nonprofit Salesforce work, including the tools below, and it will point you to whichever one matches where you are in a project.

## Featured Tools

Start with one of these if you have a live Salesforce question to answer:

| Tool | When to use it | First action |
|---|---|---|
| [NPSP Migration Readiness Scanner](https://github.com/clear-concise-carmona/npsp-migration-readiness-scanner) | You need to assess NPSP-to-Nonprofit-Cloud risk before committing to a migration timeline | Run it in a sandbox and review the blocker list before estimating work |
| [Nonprofit Data Quality Scorecard](https://github.com/clear-concise-carmona/nonprofit-data-quality-scorecard) | You need a measurable view of donor and fundraising-data conditions before or after a migration | Deploy it to a sandbox and review the first dashboard score |
| [Agentforce Nonprofit Governance Kit](https://github.com/clear-concise-carmona/agentforce-nonprofit-governance-kit) | Your organization is evaluating Agentforce and needs governance before deployment | Take the scorecard, then review policies and escalation paths with accountable staff |

## Tool Paths

### Nonprofit Migration and Data Quality

| Repo | Purpose | Audience | Best first action |
|---|---|---|---|
| [NPSP to Nonprofit Cloud Field Map](https://github.com/clear-concise-carmona/npsp-to-nonprofit-cloud-field-map) | Field-level, confidence-tagged mapping between NPSP and Nonprofit Cloud objects | Admins and architects scoping an NPSP-to-Nonprofit-Cloud migration | Read the confidence column before trusting a row, then run `validate_org.py` against your own org |
| [NPSP Migration Readiness Scanner](https://github.com/clear-concise-carmona/npsp-migration-readiness-scanner) | An `sf` CLI plugin that runs seven read-only checks and produces a 0-100 migration-readiness score | Admins and architects who need a number before committing to a migration timeline | Install the plugin and run it against a sandbox, not production |
| [Nonprofit Data Quality Scorecard](https://github.com/clear-concise-carmona/nonprofit-data-quality-scorecard) | Free Apex and Lightning Web Component package scoring 10 data-quality metrics, for either NPSP or Nonprofit Cloud | Admins and developers who want an ongoing, trackable data-quality number | Deploy to a sandbox and review the first Data Quality Dashboard score |
| [Salesforce Nonprofit Templates](https://github.com/clear-concise-carmona/salesforce-nonprofit-templates) | Downloadable templates for project scoping, data-quality audits, and Salesforce career preparation | Nonprofit admins, project managers, and career changers | Download the template that matches the work in front of you |

### AI Governance

| Repo | Purpose | Audience | Best first action |
|---|---|---|---|
| [Agentforce Nonprofit Governance Kit](https://github.com/clear-concise-carmona/agentforce-nonprofit-governance-kit) | Free 15-question AI-governance scorecard, four read-only org checks, and four forkable policy templates | Nonprofit boards, executive directors, and IT leads evaluating Agentforce | Take the scorecard first, then edit the policy templates with your board before enabling an agent |

### Salesforce Government Cloud

| Repo | Purpose | Audience | Best first action |
|---|---|---|---|
| [Awesome Salesforce Government Cloud](https://github.com/clear-concise-carmona/awesome-salesforce-government-cloud) | Curated, dated index of primary sources on Salesforce Government Cloud, including compliance, product availability, Agentforce, migration, and pricing | Public-sector buyers, architects, and implementation teams | Start here when you need a dated primary source rather than a vendor-summary answer |
| [Government Cloud Plus Migration Map](https://github.com/clear-concise-carmona/govcloud-plus-migration-map) | Field-level migration checklist and prerequisite map for Salesforce Government Cloud Plus, sourced to dated Salesforce Help documentation | Salesforce architects and public-sector teams planning a Government Cloud Plus move | Identify prerequisites and confirm each cited source against the target environment |
| [GovCloud Boundary Scanner](https://github.com/clear-concise-carmona/govcloud-boundary-scanner) | Read-only scanner for installed packages, connected apps, and Einstein/Agentforce settings against a sourced authorization dataset | Public-sector Salesforce architects and security teams | Inventory the org, then investigate each flagged boundary question with its cited source |
| [Salesforce Data Compliance Scorecard](https://github.com/clear-concise-carmona/salesforce-data-compliance-scorecard) | Read-only scorecard across 10 regulated-use configuration controls, including MFA, session policy, and classification coverage | Salesforce admins and compliance teams | Run the assessment in a sandbox and review disclosed limitations. It is not a CMMC certification tool |
| [Agentforce GovCloud Governance Kit](https://github.com/clear-concise-carmona/agentforce-govcloud-governance-kit) | Deployment templates and checklists for Agentforce in Government Cloud Plus, including permissions, field access, model pinning, and an ISSO memo | Public-sector Salesforce teams, security leads, and ISSOs | Review the authorization boundary and field-access checklist before designing an agent |

### Reference Material

| Repo | Purpose | Audience | Best first action |
|---|---|---|---|
| [Awesome Nonprofit Salesforce](https://github.com/clear-concise-carmona/awesome-nonprofit-salesforce) | Curated list of open-source Salesforce tools for nonprofits, checked weekly for maintenance status | Admins, architects, consultants, and nonprofit tech leads | Browse the category that matches your current project |

## How the Tools Fit Together

For a nonprofit migration, use the tools in the order a real project usually demands:

1. **Map the fields.** `npsp-to-nonprofit-cloud-field-map` shows what maps where and flags what nobody has confirmed yet.
2. **Score migration risk.** `npsp-migration-readiness-scanner` turns that assessment into a 0-100 score and a specific blocker list.
3. **Check the data underneath it.** `nonprofit-data-quality-scorecard` measures the data you are about to migrate. A clean migration of dirty data is still dirty data.
4. **Check AI governance before enabling anything.** `agentforce-nonprofit-governance-kit` assesses readiness for Agentforce and provides policy starting points.

For Salesforce Government Cloud work, begin with `awesome-salesforce-government-cloud` for dated primary sources. Use `govcloud-plus-migration-map` to identify prerequisites, `govcloud-boundary-scanner` to inventory authorization-boundary questions, `salesforce-data-compliance-scorecard` to review configuration posture, and `agentforce-govcloud-governance-kit` before designing an agent.

`salesforce-nonprofit-templates` runs alongside these paths for scoping, data audits, and career-preparation work. `awesome-nonprofit-salesforce` indexes these tools alongside useful work by other people.

## What to Expect

These are maintained practical tools and reference materials, not substitutes for architecture review or compliance judgment. Where a tool connects to a Salesforce org, it is designed for sandbox-first, read-only assessment. Review each repository's assumptions, confidence tags, sources, supported conditions, and disclosed limitations before relying on a result. A score or scanner can identify questions and evidence. It does not certify compliance or make an implementation decision for you.

## For Nonprofits

You don't need to read code to get value here. Start with the free [AI Readiness Scorecard](https://www.clearconciseconsulting.com/scorecard) on the Clear Concise Consulting website for a plain-language starting point. If your team has a Salesforce admin or a consultant, hand them this page. The tools here are built to run in a sandbox first and get reviewed by a person before anything changes in your live org.

## For Salesforce Admins and Consultants

Every tool here that touches a live org is read-only: describe calls, aggregate SOQL, and Tooling API queries. None of them write, update, or delete data. Run them in a sandbox, read the confidence tags and disclosed gaps in each README before you trust a result, and open an issue if a check doesn't match how migrations actually play out for you. Corrections and contributions are welcome.

## Work with Clear Concise Consulting

These tools come out of real client work: NPSP to Nonprofit Cloud migrations, data quality remediation, and AI governance assessments for nonprofits, healthcare organizations, and government agencies. If a scorecard or scan result raises questions worth talking through, see [Salesforce Nonprofit Consulting](https://www.clearconciseconsulting.com/services/salesforce-nonprofit-consulting) or start with the free [AI Readiness Scorecard](https://www.clearconciseconsulting.com/scorecard).

## Disclaimer

These are independent, open-source tools built by Clear Concise Consulting. They are not Salesforce products and are not officially affiliated with, certified by, or endorsed by Salesforce, Inc., unless a specific repo states otherwise.

## Security

Run these tools against sandboxes, not production orgs. Sample reports and scorecards in each repo use fictional or placeholder data, labeled as such. Never commit real credentials, API keys, org connection details, or client data to any repository in this account, including in issues, pull requests, or sample output. If you find a security issue in any of these tools, open an issue without posting sensitive details, or reach out through the contact page on the website.

---

Connect: [Website](https://www.clearconciseconsulting.com) · [LinkedIn](https://www.linkedin.com/in/jeremy-a-carmona/) · [Contact](https://www.clearconciseconsulting.com/contact)

Each repository carries its own license. Check before reusing.