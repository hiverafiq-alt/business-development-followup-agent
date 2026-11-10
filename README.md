# Business Development & Follow-up Agent

A private web CRM and agent workflow for research-led prospecting, stakeholder outreach and disciplined follow-up.

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/hiverafiq-alt/business-development-followup-agent)

**One click opens a prepared workspace.** You still sign in, connect your own tools and complete onboarding. Codespaces may incur charges. It is not a one-click grant of access to your email or LinkedIn.

## Start

Download or clone this repository, then run `python3 crm.py serve` with Python 3.10+. Open the private launch link printed in the terminal. No Python dependencies are required. Windows: `py crm.py serve`.

In ChatGPT Work/Codex or a tool-capable Claude environment, attach/open the repository and say:

> Read MASTER_PROMPT.md and SETUP.md. Guide me through setup, connect the tools I choose, test Telegram approvals with my own email, and operate within my recorded permissions.

## Included

- Guided onboarding, configurable stages and a private browser CRM.
- SQLite persistence; Excel `.xlsx` export with contacts, outbox and applications.
- Exact-copy and attachment approvals, Telegram preview buttons, rejection and stale-approval protection.
- Atomic send reservation, unknown-send holds, current mailbox-review requirement and company-level reply/opt-out suppression.
- Follow-up planning after 2–3 days, limited sequences and coordinated stakeholder changes.
- Product/problem/stakeholder discovery and research-led email and follow-up instructions.

## What runs where

The local application is a functioning CRM, outbox and approval bridge. Your AI host researches, writes, uses connected Apollo/Lusha/email tools and operates supported career-page browsers. This release does **not** bundle provider credentials, autonomous browser drivers, a paid AI API or a permanently running cloud agent. Live integrations require your setup and end-to-end self-test. Uncertain sends require manual reconciliation.

Read [the master workflow](MASTER_PROMPT.md), [setup and historical repairs](SETUP.md), [connector transaction contract](CONNECTORS.md) and [privacy notes](PRIVACY.md).

## Verify

`python3 -m unittest -v` tests approval invalidation, stale Telegram decisions, duplicate claims, suppression, changed attachments, delayed follow-ups, recovery and Excel output. Tests use fictional local fixtures and do not send messages.

## License

MIT for this repository's code. Connected services have their own terms and costs. This is an agent-assisted workflow, not a guarantee of interviews, replies or sales.
