<p align="center">
  <img src="assets/header.svg" alt="Sergey Yashchuk — AI workflows, MCP and automation pipelines" width="100%" />
</p>

I’m **Sergey Yashchuk**, a senior full-stack engineer (TypeScript, Node.js, React). I build tools that connect AI clients, structured data and automation workflows.

My focus is **MCP servers, automation pipelines with n8n, and developer tools**. I’m also exploring reusable **agent skills**: clear instructions, tool use and checks that make a workflow easier to repeat.

[Explore selected work](PORTFOLIO.md) · [Discuss a project](mailto:sergey.yashchuk1@gmail.com)

## Featured / MCP Lead CRM

**A lead pipeline controlled through an MCP client.**

A local TypeScript server with MCP tools, resources and a prompt for managing lead records, follow-ups and CSV files. An optional webhook connects it to n8n.

**Example:** add a lead → record a qualification score → schedule a follow-up → preview an n8n event. [Walk through the scenario](https://github.com/svtxvt/mcp-lead-crm/blob/main/docs/demo-script.md).

- **Try it locally:** fictional seed data; the local server needs no API keys.
- **Inspect the workflow:** stdio MCP calls and HTTP webhook requests are covered by tests.
- **See the limits:** the recorded webhook call is a dry run; the example email node is disabled.
- **Protocol:** built on the MCP TypeScript SDK v2; one stdio entry serves the 2026-07-28 revision and 2025-era clients. 24 tests run in CI on Node.js 20 and 22.

[Source & setup](https://github.com/svtxvt/mcp-lead-crm) · [Watch the demo](https://github.com/svtxvt/mcp-lead-crm/blob/main/docs/demo.gif) · [Tests](https://github.com/svtxvt/mcp-lead-crm/tree/main/tests)

**[n8n workflow example](https://github.com/svtxvt/mcp-lead-crm/blob/main/examples/n8n-followup-email.json)** — filters `followup_email` events and maps the event, lead ID and payload. It is inactive, with a disabled email placeholder; this starter does not include a full validation/review path.

## More engineering work

- **[Android Force 120Hz](https://github.com/svtxvt/android-force-120hz)** — a Kotlin accessibility utility for LTPO displays, with a demo and published APKs. Device compatibility and battery use remain practical trade-offs.
- **[Outhook Outbound Webhooks](https://wordpress.org/plugins/outhook-outbound-webhooks/)** — a WordPress plugin listed on wordpress.org since September 2026 after its plugin review: selected site events to n8n, Make, Zapier or any HTTPS endpoint, with optional HMAC-SHA256 signatures, a delivery log and a Docker test harness. [Source](https://github.com/svtxvt/outhook-outbound-webhooks).

## Let’s build something useful

I’m interested in collaborating on **MCP integrations, AI-assisted workflows and n8n pipelines**. I’m also exploring reusable **agent skills**. A good starting point is one concrete task, a non-sensitive sample input and a result we can check.

Available for contract work: 10–20 hours a week, remote, with 2–3 hours of daily overlap with CET.

For a small agency assignment, I offer **[one scoped n8n validation / mapping component](COLLABORATION.md)**, with sample checks and a documented handover.

**[sergey.yashchuk1@gmail.com](mailto:sergey.yashchuk1@gmail.com)**
