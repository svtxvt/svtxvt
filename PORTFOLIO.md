# Selected engineering work

Sergey Yashchuk · Senior full-stack engineer · 6+ years · TypeScript, Node.js, React

## Commercial case: collaborative workflow editor

At a US enterprise customer-service platform, a manual workflow configuration process took weeks.

I led a real-time collaborative workflow editor end to end: a React Flow canvas with Yjs CRDT over WebSocket, Redis pub/sub for horizontal scaling and MongoDB persistence. It supported 40+ node types, conditional branching and up to 10 concurrent editors.

The editor replaced the manual process with one that takes days and became a key feature in enterprise sales demos.

At the same platform, I also:

- Maintained the shared GraphQL data layer.
- Built serverless microservices and background jobs for webhooks and third-party integrations.
- Raised front-end test coverage from about 30% to 70%+.
- Mentored two junior developers.

## MCP Lead CRM

**Personal project.** A local TypeScript MCP server for lead records, activities, pipeline stages, follow-ups and CSV import/export, with an optional n8n webhook.

The JSON store uses atomic file replacement; demo seeding protects existing records. Automated tests run in [CI](https://github.com/svtxvt/mcp-lead-crm/actions/workflows/ci.yml) and cover stdio MCP calls, webhook delivery to a local receiver, concurrent writes, CSV round trips and rejected out-of-directory paths.

[Source and setup](https://github.com/svtxvt/mcp-lead-crm) · [Recorded demo](https://github.com/svtxvt/mcp-lead-crm/blob/main/docs/demo.gif) · [Walkthrough](https://github.com/svtxvt/mcp-lead-crm/blob/main/docs/demo-script.md) · [Tests](https://github.com/svtxvt/mcp-lead-crm/tree/main/tests) · [n8n starter](https://github.com/svtxvt/mcp-lead-crm/blob/main/examples/n8n-followup-email.json)

Local prototype with fictional data: the recorded webhook call is a dry run, and the inactive n8n starter has a disabled email placeholder and no credentials. SDK, protocol compatibility and test-matrix details are in the [project README](https://github.com/svtxvt/mcp-lead-crm#readme).

## Outhook Outbound Webhooks

**Personal project.** A PHP plugin that sends selected WordPress post, comment and registration events to HTTPS endpoints. It supports optional HMAC-SHA256 signatures, retries and delivery diagnostics through a delivery log and test button.

[Listed on wordpress.org](https://wordpress.org/plugins/outhook-outbound-webhooks/) since **11 September 2026**, after the plugin review. The [source](https://github.com/svtxvt/outhook-outbound-webhooks) includes [quality notes](https://github.com/svtxvt/outhook-outbound-webhooks/blob/main/QUALITY-NOTES.md) recording Plugin Check, PHPCS and signed-request checks, plus a [Docker end-to-end harness](https://github.com/svtxvt/outhook-outbound-webhooks/blob/main/dev/e2e.sh) with a signature-verifying receiver.

## Android Force 120Hz

**Personal project.** A Kotlin accessibility utility for Android LTPO displays that lower their refresh rate on static content. It animates a small overlay and provides startup controls; the repository documents installation, signing and OEM battery/autostart settings.

**1,179 APK downloads across two releases, as of 6 September 2026.**

[Source](https://github.com/svtxvt/android-force-120hz) · [Demo](https://github.com/svtxvt/android-force-120hz#demo) · [APK releases](https://github.com/svtxvt/android-force-120hz/releases)

Device compatibility and battery use vary. Licensed under CC BY-NC-SA 4.0, including its non-commercial restriction.

**Build status, 6 September 2026:** the release workflow was failing at that check.

## Collaboration

Available for [part-time AI integration contracts](COLLABORATION.md): 10–20 hours/week, in fixed working slots with 2–3 hours of daily CET/CEST overlap.

**[sergey.yashchuk1@gmail.com](mailto:sergey.yashchuk1@gmail.com)** · [Profile](README.md)
