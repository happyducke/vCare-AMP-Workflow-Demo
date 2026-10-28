vCare AMP - two-week team handoff
Updated October 28, 2026

Shareable demo: https://happyducke.github.io/vCare-AMP-Workflow-Demo/
Plan: https://happyducke.github.io/vCare-AMP-Workflow-Demo/vCare_AMP_Implementation_Plan.pdf
Team ZIP: https://happyducke.github.io/vCare-AMP-Workflow-Demo/vCare_AMP_Team_Handoff.zip
Source: https://github.com/happyducke/vCare-AMP-Workflow-Demo

TARGET AND STACK
10 business days to a controlled production pilot; two developers using AI,
part-time Operations/QA, same-day decisions and repository/AWS access on Day 1.
PC plus USB keyboard-input scanner only; Enter/Tab. Extend AMP's existing
backend, database, login and AWS pipeline. Day 3 staging; Day 10 pilot.
The PDF has four implementation/release pages and three UI previews.
The Markdown plan is editable; four copy-ready prompts are included.

TRY THE ACTIVE PACK JOB (ABOUT TWO MINUTES)
1. Open the shared demo or vCare_AMP_Proposed_UI.html in a desktop browser.
   Start with Production Lead. Open Prototype Guide / Reset demo if needed.
2. Pack Jobs > New Pack Job. Choose Quick Scanner Demo Kit (3 scans),
   target quantity 1, and an optional production reference. Create the job.
3. Scan/type 020000000006, then Enter/Tab or Add controller. It must be a
   registered controller with matching SKU and no previous assignment.
   The detail page also provides registered sample Controller buttons.
4. Open packing. Scan 99G33-19B73C6, then PC71-RADINTC-10M, then
   DEMO-PACK-LABEL. The same codes are clickable in the demo helper.
   The primary and equivalent share required quantity 2; a third is blocked.
5. Save progress and reload to try resume. Confirm packing/seal, then
   Verify & Mark Ready. Ready Inventory shows the acting verifier and time.
6. Switch to Sales Admin. New Shipment uses existing Customer/Site dropdowns,
   SO, PO and target date. Scan that Ready Controller MAC or select it from
   Ready Inventory. SKU/checklist/packing evidence and quantities attach
   automatically. Enter actual ship date, confirm dispatch, then Export Excel.

For a second controller use 020000000007 and a target quantity of 2.
Every new controller starts at zero and retains its own scans. The short kit
is explicitly demo-only; full supplied checklist configurations are available.
Duplicate/unknown/wrong-SKU controllers and job over-capacity are rejected.
Save progress uses this browser's local storage. Viewers do not share data.
Reset demo clears only this demo's saved state. The role selector demonstrates
permissions; it is not authentication. No production API is connected.

OTHER WORKFLOWS
- Justin can view all shipments, search SO/PO/customer/site/MAC and sort/filter.
- Shipment creation requires no manual lines, SKU, checklist or packing list.
- Only confirmed Ready, sealed, unheld, unallocated controllers can be added.
- Different checklist configurations stay distinct even for the same SKU.
- New Shipment Checklist creates a separate identity at R1, blank or copied.
  Draft editing and Operations approval are separate from creating revisions.
- Primary/equivalent quantities combine; actual scanned P/Ns remain recorded.
- Taiwan original serials remain; differences require a recorded review.
- Ready verifier/time link to sign-off history. Reopening requires fresh sign-off.

CONTENTS
Implementation Plan PDF/Markdown; four AI prompts; functional standalone HTML;
this README; sample shipment XLSX; ui_previews/ including new job form/details.
Keep ui_previews/ beside the editable plan for image references.
Sample XLSX shows the same SKU with different packing configurations, tracking
blocks and a filterable unit tab. MAC/SO/PO remain text; dates remain dates.
Draft exports show allocation; confirmed exports use retained dispatch evidence.

VERIFICATION COMPLETED ON THE PROTOTYPE
- Created a two-controller job; duplicate and wrong-SKU MACs were rejected.
- Primary + equivalent fulfilled a shared quantity; excess scans were rejected.
- Progress survived reload; the second controller retained separate zero counts.
- Seal/verification moved both controllers to Ready with named verifier/time.
- Scanned one into a new shipment and selected the second from Ready Inventory.
- Dispatched both; exported XLSX reopened with quantity 2 and both exact MACs.
- Job progress updated to Complete with two shipped controllers; no browser errors.
Earlier checks covered customer/site validation, non-Ready/duplicate allocation,
mixed checklist exports, independent checklist creation/revisions, equivalent-only
completion, verifier history and reopening. These are prototype checks, not
production AMP acceptance. Run the six release checks with the actual scanner.

PUBLICATION AND PRODUCTION
GitHub Pages hosts the static demonstration and shareable downloads.
The plan describes AWS production deployment; no AWS resources are provisioned.
Only illustrative prototype data and handoff artifacts are published. Meeting
recordings, original attachments and production screenshots are not included.
