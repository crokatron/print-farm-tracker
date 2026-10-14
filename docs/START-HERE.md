# 3D Print Farm Tracker: start here

**Continuing this tool? Read [the detailed handover](HANDOVER.md).** For pictures and operation, use the [manual](USER-MANUAL.md) and [offline demo](../demo.html).

Tracks requests, quantities, instructions, print status and QC decisions. It is an independent operational tracker, not Parts Bench or a printer-control service.

**Start with:** Record a request. Choose + New Request. Enter the requester and part details, quantity and due date. Pasting an email keeps it as reference; fill the structured fields yourself.

**Source:** this is a private source checkpoint, not a live-system mirror. Check [the source manifest](../SOURCE-MANIFEST.json) and current working files before merging.

**Keep your work safe:** Browser storage and an explicitly connected folder are distinct. Recheck the saving indicator when reopening the tool; browser permissions may need renewal. CSV is a summary and should not be assumed to contain every photo or detailed field.

**Next maintainer action:** Create a fictional request, change status/QC, save and reopen in the actual folder-backed mode. Confirm attachment recovery and reporting. Do not interpret a Printing status label as a machine command.

**Status:** private upload verified on 14 October 2026. These guides accompany the private source package. Live runtime, data backups and full recovery were not retested. Public release needs separate approval.
