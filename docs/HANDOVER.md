# 3D Print Farm Tracker: maintainer handover

[One-screen summary](START-HERE.md) · [User manual](USER-MANUAL.md) · [Feature overview](../README.md) · [Recorded validation](../VALIDATION.md)

## Purpose and behaviour to preserve

Track a print request from intake through production, quality checks and delivery. This browser tool records who asked for a part, the agreed printing instructions and the result, and can generate a traceability report. It does not slice models or launch printers.

- **Intake:** Requester, part, quantity, date, notes and an optional pasted request email. (Request lifecycle.)
- **Team instructions:** Material, colour, machine, layer height, infill, temperature, priority and finishing requirements. (Request lifecycle.)
- **Status:** New, Instructions Ready, Printing, QC, Completed, Delivered and On Hold. (Request lifecycle.)
- **Production and QC:** Produced quantity, pass/rework/reprint result, notes, operator/date and a finished-part photo. (Request lifecycle.)
- **Reports:** Generate a traceability report for print/PDF and export a CSV job log. (Request lifecycle.)
- **Folder storage:** Connect a data folder when browser support and permission allow it. (Request lifecycle.)

The [demo](../demo.html) is a smaller, labelled simulation with fictional data. It explains cause and effect without the real service; it is not evidence of a working production installation. Numbered screenshots in the user manual distinguish actual-app captures from demo captures.

## Files and sources of truth

| Actual package path | Maintainer role |
| --- | --- |
| [external-sources/StandaloneTools/3D_Print_Farm_Tracker.html](../external-sources/StandaloneTools/3D_Print_Farm_Tracker.html) | Single-file request tracker |
| [demo-source](../demo-source) | Editable demo HTML/CSS/runtime and embedded screenshot tour |
| [SOURCE-MANIFEST.json](../SOURCE-MANIFEST.json) | Original copied-source paths and SHA-256 checkpoint values |

The original working source is under C:/Users/lamon/Desktop/AI TOOLS/NAS for NAS modules; adjacent CAD/watch source locations are recorded by the full backup’s reviewed source manifest. This package contains only the explicitly copied source, not an automatic mirror. The main private nas-projects backup retains the broader shared host context.

## Setup, run and tests

Run commands from this repository root unless a `cd` is shown. Use a disposable checkout and fictional data for first setup. Dependencies, SDKs, signing material and personal data are not bundled. The following are continuation instructions grounded in the retained source, **not commands executed or newly certified by this handover**.

```powershell
python -m http.server 8765 --bind 127.0.0.1
```

/external-sources/StandaloneTools/3D_Print_Farm_Tracker.html

Selected project check:

No independent automated production test suite is included for this module/single-file package. Use the project-specific checks below and the shared host test suite where applicable; do not invent an `npm test` command.

For the documentation demo alone, serve this repository on loopback with `python -m http.server 8765 --bind 127.0.0.1` and open `/demo.html`. Choose a free port if another preview is running. JavaScript syntax can be checked with `node --check demo-source/runtime.js`. `python demo-source/rebuild.py` rewrites demo.html, so run it only in a disposable checkout or an authorised demo-editing session. A local server cannot provide missing HA/CAD/NAS functions. Inspect browser tests for installed dependencies, fixture requirements and network targets before running them with the approved browser tooling.

## Data, configuration and backup boundaries

Browser storage and a user-connected folder are distinct. Folder permissions can expire; inspect the saving indicator after reopening. Back up detailed request data and attachments, not only summary CSV.

Browser storage and an explicitly connected folder are distinct. Recheck the saving indicator when reopening the tool; browser permissions may need renewal. CSV is a summary and should not be assumed to contain every photo or detailed field.

Git preserves reviewed source and documentation. It does not copy browser storage, application databases, uploaded models/photos, accepted device settings, SDKs or credentials. Maintain independent recovery copies of the data identified above, including matching configuration and asset versions. Never add real secrets to examples, issues or logs. Private source copies on GitHub are not proof of a complete NAS/offsite data backup.

## Current verification and Git state

Before these documentation edits on 14 October 2026, this package was clean on branch `main` at `c0f0e8caffa7594af23a4e9ffff48dfcd2ebb2fa` and its private upload was verified. All 1 manifest-listed source entries matched their stored checksums before editing. The upload follow-up has completed all 17 repositories and is paused; it does not run this tool or back up its live data.

These handover pages and README links accompany the private source package. Preserve them when continuing; stage only reviewed changes. Recheck current `git status --short --branch` and `git diff` before starting. No project-specific background schedule was inspected or changed in this documentation pass. Any service schedules in older notes are historical claims to verify in the actual deployment.

Earlier package checks and limits are recorded in [VALIDATION.md](../VALIDATION.md). This handover adds documentation/link/whitespace/secret and source-preservation checks only. No current NAS release, real hardware state, fresh installation, complete data restoration or offsite-backup freshness was verified here.

## Recovery approach

1. Preserve the current installation/data before changing it. Identify the exact code commit and data snapshot required; do not assume this package matches the running service.
2. Recover source into a new folder. Verify the source manifest and restore the project-specific configuration/assets described above separately. Recreate dependencies from the retained project files and guides.
3. Restore user data into an isolated instance or clean test browser. Check a representative editable record, associated files and save/reload behaviour, then compare to the original. Do not test recovery by overwriting production.
4. Record what actually restored and what remains missing. A demo opening or a passing syntax check is not a production recovery drill. Real deployment/device actions need the existing authorised workflow.

## Known limits and next work

The screenshot contains a fictional request. No real requester details were copied. This tracker is independent of Parts Bench and does not imply automatic printer communication.

**Priority:** Create a fictional request, change status/QC, save and reopen in the actual folder-backed mode. Confirm attachment recovery and reporting. Do not interpret a Printing status label as a machine command.

Common symptoms to check for this tool:

- No folder saving: connect the intended folder using a browser with the required file-system support.
- Request missing: clear search/status filters and check browser/site storage.
- Report incomplete: save instructions and production information before regenerating it.

Keep [the release checklist](../RELEASE-CHECKLIST.md) and [third-party notes](../THIRD-PARTY.md) with the package. Original contributions use MIT; bundled/upstream code and assets keep their own licences. Public publication is a separate decision; preparing documentation is not permission to publish.
