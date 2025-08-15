# DirectCare
DirectCare
Tools, templates, and automations for direct-to-employer healthcare contracting—from bundled pricing and care navigation to claims recovery and payment workflows. Built to be practical, fast, and vendor-agnostic.

Short version: this is where we keep the stuff that saves purchasers money and saves everyone else a headache.

Contents (current & planned)
bash
Copy
Edit
/docs/                Strategy notes, playbooks, one-pagers (no PHI)
/proposals/           Buyer/provider proposal templates & case studies
/pricing/             Public pricing references & benchmarks (no PHI)
/automation/          Scripts & macros (Python, VBA, PowerShell)
/dashboards/          Looker/Sheets specs & data definitions
/crm/                 Data dictionaries, import/export mappings
/legal/               Agreement templates & BAAs (public-safe only)
/ops/                 SOPs for outreach, navigation, settlements
Data policy: No PHI, no member-identifiable data, no payer-confidential rate sheets. Use redacted samples only.

Getting started
1) Clone
bash
Copy
Edit
git clone https://github.com/gstek-alt/DirectCare.git
cd DirectCare
2) (Optional) Python environment
powershell
Copy
Edit
# Windows PowerShell
py -3.11 -m venv .venv
. .\.venv\Scripts\Activate.ps1
python -m pip install -U pip
pip install -r automation/requirements.txt
3) Pre-commit (optional but recommended)
bash
Copy
Edit
pip install pre-commit
pre-commit install
Conventions
Branches: feat/<short-name>, fix/<short-name>, ops/<short-name>

Commits: Imperative, present tense — e.g., add gramercy bundled pricing template

PRs: Keep small; include a short “why” and a before/after if relevant

Secrets: Never commit API keys, access tokens, or live credentials. Use .env (git-ignored) and local machine secrets.

Useful entry points
automation/

excel/ — Outlook/Excel VBA (e.g., SRFax, email merge)

python/ — Parsing, pricing, and claims QC helpers

docs/one-pagers/ — Provider & purchaser one-pagers

proposals/ — Program outlines and buyer decks (export-only)

Roadmap
 Starter templates for ASC bundled pricing (ortho/MSK focus)

 Scripts to normalize claims CSVs and flag SOC shift opportunities

 SRFax status checker + Excel log updater

 Zoho import/export mappers (Accounts, Contacts, Deals)

 Looker/Sheets spec for settlement tracking dashboard

 “How to Use” member flyer generator (NYC providers first)

If you’re here to contribute: open an issue with context, then a PR. Low ceremony, high clarity.

License
Private repository — All rights reserved. Ask before sharing outside the team.

Contact
Gavin Steketee (G)
President, DirectCare
gstek@directcarenet.com • 913-671-0893 • https://directcarenyc.com

