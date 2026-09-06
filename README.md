<p align="center">
  <img src="assets/header.svg" alt="Sergey Yashchuk — AI workflows, MCP and automation pipelines" width="100%" />
</p>

I’m **Sergey Yashchuk**, a software engineer and **AI enthusiast**. I build tools that connect AI clients, structured data and automation workflows.

My focus is **MCP servers, automation pipelines with n8n, and developer tools**. I’m also exploring reusable **agent skills**: clear instructions, tool use and checks that make a workflow easier to repeat.

[Explore selected work](PORTFOLIO.md) · [Discuss a project](mailto:sergey.yashchuk1@gmail.com)

## Featured / MCP Lead CRM

**A lead pipeline controlled through an MCP client.**

A local TypeScript server with MCP tools, resources and a prompt for managing lead records, follow-ups and CSV files. An optional webhook connects it to n8n.

**Example:** add a lead → record a qualification score → schedule a follow-up → preview an n8n event. [Walk through the scenario](https://github.com/svtxvt/mcp-lead-crm/blob/main/docs/demo-script.md).

- **Try it locally:** fictional seed data; the local server needs no API keys.
- **Inspect the workflow:** stdio MCP calls and HTTP webhook requests are covered by tests.
- **See the limits:** the recorded webhook call is a dry run; the example email node is disabled.

[Source & setup](https://github.com/svtxvt/mcp-lead-crm) · [Watch the demo](https://github.com/svtxvt/mcp-lead-crm/blob/main/docs/demo.gif) · [Tests](https://github.com/svtxvt/mcp-lead-crm/tree/main/tests)

**[n8n workflow example](https://github.com/svtxvt/mcp-lead-crm/blob/main/examples/n8n-followup-email.json)** — filters `followup_email` events and maps the event, lead ID and payload. It is inactive, with a disabled email placeholder; this starter does not include a full validation/review path.

## More engineering work

- **[Android Force 120Hz](https://github.com/svtxvt/android-force-120hz)** — a Kotlin accessibility utility for LTPO displays, with a demo and published APKs. Device compatibility and battery use remain practical trade-offs.
- **[Simple Outbound Webhooks](https://github.com/svtxvt/simple-outbound-webhooks)** — an event-to-HTTPS integration for WordPress, with optional HMAC signatures, a delivery log and a Docker test harness.

## Let’s build something useful

I’m interested in collaborating on **MCP integrations, AI-assisted workflows and n8n pipelines**. I’m also exploring reusable **agent skills**. A good starting point is one concrete task, a non-sensitive sample input and a result we can check.

For a small agency assignment, I offer **[one scoped n8n validation / mapping component](COLLABORATION.md)**, with sample checks and a documented handover.

**[sergey.yashchuk1@gmail.com](mailto:sergey.yashchuk1@gmail.com)**
