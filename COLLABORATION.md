# One small component for an existing n8n workflow

A first assignment can be one agreed data-validation or field-mapping component. Useful when your team already owns the integration and wants to hand over a clearly defined piece of implementation.

## Example task

Take one agreed JSON input format, check the required fields, and map valid records to one agreed output schema. Route records needing review with a reason. The rules come from your specification; this is a proposed assignment, not a ready-made universal validator.

## What you receive

- Workflow JSON for the agreed n8n version.
- Synthetic test inputs, expected outputs and recorded check results.
- A short import/setup guide and one revision within the agreed scope.

Fixes needed to pass the agreed acceptance cases are included; the revision is one additional change request within the same agreed scope.

Before work starts, we agree the input/output contract, acceptance cases (including normal, invalid and missing-field input), delivery date and payment terms. Your team connects credentials, integrates the component and deploys it. Live CRM integration, hosting and ongoing support are outside this component.

## Work you can inspect

My [MCP Lead CRM](https://github.com/svtxvt/mcp-lead-crm) shows TypeScript MCP tools, structured records, CSV handling and an optional n8n webhook, with a [demo](https://github.com/svtxvt/mcp-lead-crm/blob/main/docs/demo.gif) and [tests](https://github.com/svtxvt/mcp-lead-crm/tree/main/tests). It is a local prototype; the recorded webhook is a dry run. It demonstrates related integration work, not a completed client n8n deployment.

The public [n8n starter JSON](https://github.com/svtxvt/mcp-lead-crm/blob/main/examples/n8n-followup-email.json) shows event filtering and payload mapping. It is inactive, with a disabled email placeholder; it does not implement a complete validation/review path. An existing synthetic conditional/mapping example with a mock HTTP handoff is also available on request.

## Start with a short description

Tell me the input, the expected result and your n8n version. A brief description is enough to check fit; use synthetic examples when we agree the details. Please leave out credentials and customer data.

**[sergey.yashchuk1@gmail.com](mailto:sergey.yashchuk1@gmail.com)**

Price and delivery are confirmed for the agreed scope. Other MCP and AI-workflow projects are scoped separately.

[Profile](README.md) · [Selected work](PORTFOLIO.md)
