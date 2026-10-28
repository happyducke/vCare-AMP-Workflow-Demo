# vCare AMP workflow demo

[Open the interactive demo](https://happyducke.github.io/vCare-AMP-Workflow-Demo/) · [Implementation plan](https://happyducke.github.io/vCare-AMP-Workflow-Demo/vCare_AMP_Implementation_Plan.pdf) · [Download team package](https://happyducke.github.io/vCare-AMP-Workflow-Demo/vCare_AMP_Team_Handoff.zip)

Updated October 28, 2026. Proposed AMP extension with a two-week implementation plan, AI build prompts, AWS release steps, sample Excel export and UI previews.

## Try the flow

1. Start as **Production Lead**. Packaging → **New Pack Job** → **Quick Scanner Demo Kit (3 scans)** → target quantity **1** → create.
2. Add Controller MAC **020000000006** and open packing.
3. Scan/type **99G33-19B73C6**, **PC71-RADINTC-10M**, then **DEMO-PACK-LABEL**, or use the three sample buttons. Primary and equivalent parts share the required quantity. USB keyboard-input scanners support Enter/Tab.
4. Save progress to try resume. Confirm the sealed contents and **Verify & Mark Ready**. Ready Inventory retains the verifier and time.
5. Switch to **Sales Admin**, create a shipment with existing Customer/Site, SO/PO and target date, then scan/select the Ready controller. Enter actual ship date, dispatch and export Excel.

For two units set target 2 and also add **020000000007**. Each has separate scan counts. Unknown, duplicate, wrong-SKU and over-capacity controller additions are rejected. Read [the handoff instructions](vCare_AMP_Handoff_README.txt) for details.

## Scope

Static interactive prototype with illustrative data. Each viewer saves their own progress in their browser; there is no shared production backend. Reset demo is in Prototype Guide. The role selector demonstrates workflow and is not authentication. The quick kit is demo-only; full checklist examples remain available. No AWS resources are provisioned by this repository. The plan describes extending the existing AMP backend, database, auth and AWS pipeline over 10 business days.

Only prototype and team handoff files are published. Original meeting media, attachments and production AMP screenshots are excluded.

## Local use

Download the team ZIP, extract it, and open `vCare_AMP_Proposed_UI.html` in a desktop browser. Keep `ui_previews/` beside the editable plan. GitHub Pages publishes from the root of `main`; `.nojekyll` serves the static files directly.
