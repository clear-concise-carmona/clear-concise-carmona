# Clear Concise Consulting

Open source Salesforce tools for nonprofits, built from real migration, data quality, and AI governance work.

Clear Concise Consulting is a Salesforce consulting practice founded by Jeremy Carmona, who has 14 years of hands-on Salesforce experience starting in 2012 at Environmental Defense Fund, holds 13 Salesforce certifications, and has taught Salesforce Administration at NYU Tandon School of Engineering. The practice works with nonprofits, healthcare organizations, and government agencies on Salesforce implementation, data governance, and AI governance. Assumptions aren't facts, so these tools are built to say "we don't know yet" instead of guessing, and every claim carries a source or a confidence tag.

Website: [clearconciseconsulting.com](https://www.clearconciseconsulting.com)

---

## Start Here

New to this account? Start with [awesome-nonprofit-salesforce](https://github.com/clear-concise-carmona/awesome-nonprofit-salesforce). It's a curated, weekly-checked list of open source tools for nonprofit Salesforce work, including the five tools below, and it will point you to whichever one matches where you are in a project.

## The Tools

| Repo | Purpose | Audience | Best First Action |
|---|---|---|---|
| [awesome-nonprofit-salesforce](https://github.com/clear-concise-carmona/awesome-nonprofit-salesforce) | Curated list of open source Salesforce tools for nonprofits, checked weekly for maintenance status | Admins, architects, consultants, nonprofit tech leads | Browse the list and find the category that matches your current project |
| [npsp-to-nonprofit-cloud-field-map](https://github.com/clear-concise-carmona/npsp-to-nonprofit-cloud-field-map) | Field-level, confidence-tagged mapping between NPSP and Nonprofit Cloud objects | Admins and architects scoping an NPSP to Nonprofit Cloud migration | Read the confidence column before trusting a row, then run `validate_org.py` against your own org |
| [npsp-migration-readiness-scanner](https://github.com/clear-concise-carmona/npsp-migration-readiness-scanner) | An `sf` CLI plugin that runs seven read-only checks and produces a 0-100 migration readiness score | Admins and architects who need a number before committing to a migration timeline | Install the plugin and run it against a sandbox, not production |
| [nonprofit-data-quality-scorecard](https://github.com/clear-concise-carmona/nonprofit-data-quality-scorecard) | Free Apex and Lightning Web Component package scoring 10 data quality metrics, works with either NPSP or Nonprofit Cloud | Admins and developers who want an ongoing, trackable data quality number | Deploy to a sandbox and review your first Data Quality Dashboard score |
| [agentforce-nonprofit-governance-kit](https://github.com/clear-concise-carmona/agentforce-nonprofit-governance-kit) | Free 15-question AI governance scorecard plus four read-only org checks and four forkable policy templates | Nonprofit boards, executive directors, and IT leads evaluating Agentforce | Take the free scorecard first, then edit the policy templates with your board before enabling any agent |
| [salesforce-nonprofit-templates](https://github.com/clear-concise-carmona/salesforce-nonprofit-templates) | Downloadable templates for project scoping, data quality audits, and Salesforce career prep | Nonprofit admins, project managers, and career changers | Download the template that matches what you're working on today |

## How the Tools Fit Together

These tools follow the order a real NPSP to Nonprofit Cloud project actually happens in:

1. **Map the fields.** `npsp-to-nonprofit-cloud-field-map` shows what maps where, and flags what nobody has confirmed yet.
2. **Score the migration risk.** `npsp-migration-readiness-scanner` turns that mapping into a 0-100 score and a specific blocker list for your org.
3. **Check the data underneath it.** `nonprofit-data-quality-scorecard` scores the data you're about to migrate, since a clean migration of dirty data is still dirty data.
4. **Check AI governance before turning anything on.** `agentforce-nonprofit-governance-kit` scores whether your org is ready for Agentforce, using the same gate definitions Clear Concise Consulting uses in paid engagements.

`salesforce-nonprofit-templates` runs alongside this chain rather than inside it. It covers scoping, data audits, and career prep work that doesn't require a live org.

`awesome-nonprofit-salesforce` indexes all of it, plus tools built by other people.

## For Nonprofits

You don't need to read code to get value here. Start with the free [AI Readiness Scorecard](https://www.clearconciseconsulting.com/scorecard) on the Clear Concise Consulting website for a plain-language starting point. If your team has a Salesforce admin or a consultant, hand them this page. The tools here are built to run in a sandbox first and get reviewed by a person before anything changes in your live org.

## For Salesforce Admins and Consultants

Every tool here that touches a live org is read-only: describe calls, aggregate SOQL, and Tooling API queries. None of them write, update, or delete data. Run them in a sandbox, read the confidence tags and disclosed gaps in each README before you trust a result, and open an issue if a check doesn't match how migrations actually play out for you. Corrections and contributions are welcome.

## Work with Clear Concise Consulting

These tools come out of real client work: NPSP to Nonprofit Cloud migrations, data quality remediation, and AI governance assessments for nonprofits, healthcare organizations, and government agencies. If a scorecard or scan result raises questions worth talking through, see [Salesforce Nonprofit Consulting](https://www.clearconciseconsulting.com/services/salesforce-nonprofit-consulting) or start with the free [AI Readiness Scorecard](https://www.clearconciseconsulting.com/scorecard).

## Disclaimer

These are independent, open source tools built by Clear Concise Consulting. They are not Salesforce products and are not officially affiliated with, certified by, or endorsed by Salesforce, Inc., unless a specific repo states otherwise.

## Security

Run these tools against sandboxes, not production orgs. Sample reports and scorecards in each repo use fictional or placeholder data, labeled as such. Never commit real credentials, API keys, org connection details, or client data to any repo in this account, including in issues, pull requests, or sample output. If you find a security issue in any of these tools, open an issue without posting sensitive details, or reach out through the contact page on the website.

---

Connect: [Website](https://www.clearconciseconsulting.com) · [LinkedIn](https://www.linkedin.com/in/jeremy-a-carmona/) · [Contact](https://www.clearconciseconsulting.com/contact)

Each repo carries its own license. Check before reusing.
