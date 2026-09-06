# AI tools, workflows & selected engineering

Public work by Sergey Yashchuk ([svtxvt](https://github.com/svtxvt)), a software engineer and AI enthusiast. My current focus is MCP integrations, automation pipelines and reusable agent skills. MCP Lead CRM is the main public example of that direction; the other projects show my broader engineering experience. Each case links to implementation and evidence you can inspect.

## MCP Lead CRM

**Problem.** A small lead pipeline needs structured records and follow-ups that an MCP client can work with, without first setting up a hosted CRM.

**Implementation.** I built a local TypeScript MCP server with tools for leads, activities, pipeline stages, due follow-ups, CSV import/export and an optional n8n webhook. Data lives in a JSON store. CSV paths are confined to the data directory, writes use atomic replacement, and the demo seed refuses to overwrite a non-empty store unless explicitly requested.

**Evidence.** The repository includes [source and installation steps](https://github.com/svtxvt/mcp-lead-crm), a [recorded demo](https://github.com/svtxvt/mcp-lead-crm/blob/main/docs/demo.gif), a [walkthrough](https://github.com/svtxvt/mcp-lead-crm/blob/main/docs/demo-script.md) and [tests](https://github.com/svtxvt/mcp-lead-crm/tree/main/tests).

**Verification, 6 September 2026.** A fresh checkout of commit `36450af06b7bee2a5a51a6b5df34d7c1a45d9021` passed `npm ci` and all **21 tests in 5 files** with Node.js 22.22.2. The tests include stdio MCP calls and HTTP webhook requests to a local receiver. This is a local test result; the repository did not yet have a CI workflow at that commit.

**Scope.** This is a local integration prototype with fictional demo records. The recorded webhook call is a dry run; the example email node is disabled. It does not establish a customer deployment or a paid business result. MIT licensed.

## Android Force 120Hz

**Problem.** Some Android LTPO displays reduce their refresh rate on static content even when a user requests a higher rate through settings or ADB.

**Implementation.** I built a Kotlin app with an accessibility service that animates a small overlay, plus controls for startup stability after reboot. The repository explains installation, signing and OEM-specific battery/autostart settings.

**Evidence.** There is a [demonstration](https://github.com/svtxvt/android-force-120hz#demo), [source](https://github.com/svtxvt/android-force-120hz), and [two published APK releases](https://github.com/svtxvt/android-force-120hz/releases). GitHub reported **1,179 APK asset downloads** across v1.0.0 and v1.1.0 on **6 September 2026** (57 + 1,122). This is a download count, not a count of users or successful installations.

**Scope.** Behaviour depends on the device and OEM; maintaining a higher refresh rate uses more battery. Source contains Robolectric tests, but the current published release workflow is failing, so a passing CI build is not claimed. The license is **CC BY-NC-SA 4.0**, including its non-commercial restriction.

## Simple Outbound Webhooks

**Problem.** WordPress site events need to reach an external workflow through a small, inspectable integration.

**Implementation.** I built a PHP plugin for selected post, comment and registration events. It sends JSON to configured HTTPS endpoints, supports an optional HMAC-SHA256 signature, and includes a delivery log, test button and developer filters. The signed message combines a timestamp with the raw request body so the receiving service can verify it.

**Evidence.** The public repository includes [the plugin](https://github.com/svtxvt/simple-outbound-webhooks), a distributable ZIP, [quality notes](https://github.com/svtxvt/simple-outbound-webhooks/blob/main/QUALITY-NOTES.md) and a [Docker end-to-end harness](https://github.com/svtxvt/simple-outbound-webhooks/blob/main/dev/e2e.sh) with a signature-verifying receiver. The notes record Plugin Check, PHPCS and signed-request checks.

**Scope.** These are repository verification artifacts, not customer adoption figures. A public repository or ZIP does not mean approval in the WordPress plugin directory. GPL-2.0-or-later.

---

## Collaboration

I’m interested in collaborating on MCP integrations, AI-assisted workflows, automation pipelines and reusable agent skills. I prefer a focused task with a clear acceptance check and a handover someone else can run.

Send a short description, a non-sensitive sample input and the expected output to **[sergey.yashchuk1@gmail.com](mailto:sergey.yashchuk1@gmail.com)**. We can agree scope, delivery and payment terms before starting.

[Back to profile](README.md)
