# 3D Print Farm Tracker — visual user manual

[Project overview](../README.md) · [Offline interactive demo](../demo.html)

Start with the numbered picture guide. Each number identifies the exact highlighted control. Work through one step at a time; the longer reference is below it.

### Actual tool · controls at a glance

Actual application screenshot. Numbered boxes point to the controls described below. 

![3D Print Farm Tracker — numbered controls](images/guide-1.jpg)

1. **Track the real stage.** Move from New through production, QC and delivery as the work happens.
2. **Record print instructions.** Choose material and save the agreed production settings below.
3. **Check where records save.** Connect the intended folder and confirm the saving indicator.

### Try the working offline example

Screenshot of this project’s interactive demo. Side-by-side services are explicitly simulated.

![3D Print Farm Tracker — numbered controls](images/guide-2.jpg)

1. **Name the requested part.** Keep a clear request identity and quantity.
2. **Record the actual result.** Status and quality result describe different things.
3. **Check the saved record.** The dummy request keeps your edits without launching a printer.

## Detailed task reference

### Record a request

1. Choose + New Request. Enter the requester and part details, quantity and due date. Pasting an email keeps it as reference; fill the structured fields yourself.
2. Choose Save Request and note the REQ identifier. Use that identifier in team communications so similarly named parts are not confused.
3. Complete Instructions for Team, including machine, material, layer height and any tolerances/finishing. Save Instructions before changing status.

### Track production and quality

1. Move the request to Instructions Ready when instructions are agreed, then Printing when production actually begins. The status itself does not start a machine.
2. Record actual quantity produced, QC result, notes and who completed the work. Add a photo if appropriate and Save Production Info.
3. Use Fail - reprint or Fail - rework when that is the result. Do not mark Delivered merely because printing finished.

### Export and retain the job record

1. Generate Traceability Report and review requester, part, print specifications and QC information before Print / Save PDF.
2. Export the CSV job log for a summary across requests; the detailed report is a separate artifact.
3. Use Connect data folder if supported and confirm the saving status. The page explicitly says Not saving to a folder when no folder is connected.

## Keep your work

Browser storage and an explicitly connected folder are distinct. Recheck the saving indicator when reopening the tool; browser permissions may need renewal. CSV is a summary and should not be assumed to contain every photo or detailed field.

## If something looks wrong

- No folder saving: connect the intended folder using a browser with the required file-system support.
- Request missing: clear search/status filters and check browser/site storage.
- Report incomplete: save instructions and production information before regenerating it.

## What this manual does not promise

The screenshot contains a fictional request. No real requester details were copied. This tracker is independent of Parts Bench and does not imply automatic printer communication.

Screenshots show the actual application where captured. The offline demo is a deliberately smaller simulation and identifies its dummy services. It never controls devices, sends notifications, uploads files or launches printing.
