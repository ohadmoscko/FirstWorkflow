## Learn More (Full Docs)
# FirstWorkflow – Secure Webhook Form

Single-file HTML page that posts quotes to a Make.com webhook. Enter your **Webhook URL** and **Secret** once, click **Save Config** (stored locally in your browser), then use **Send Test Ping** or **Request a Quote**.  
Make scenario validates the secret and writes rows to **FirstWorkflow_Quotes / Sheet1** in Google Sheets.  
> Do **not** hard-code secrets in the HTML; the page stores them only in localStorage on your device.

**Live (GitHub Pages):** Settings → Pages → Deploy from branch → `main` / root, then visit `https://<your-username>.github.io/FirstWorkflow/`.
Field alignment: the page sends `name`, `scope`, `ts` to match the Make mapping.


For full documentation (prompts, outputs, changelog, history), see:
👉 https://github.com/ohadmoscko/GPT-backups


# FirstWorkflow – AI Agent Demo

This repository hosts the **live demo** of the AI Agent Workflow project.
It shows how a team of specialized AI agents (Ideas, Strategy, Risk, Documentation, Packaging, etc.) collaborate step by step.

## Features
- Single-file HTML app (`index.html`)
- Visual workflow of agents
- Simple example case study (manual → automated handoffs)

## Learn More (Full Docs)
For full documentation (prompts, outputs, changelog, history), see:
👉 https://github.com/ohadmoscko/GPT-backups

## Screenshot
![Workflow](assets/screenshots/workflow.png)

## License
MIT (see [LICENSE](./LICENSE))
