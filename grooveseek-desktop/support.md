# GrooveSeekDesktop Support

> **日本語版**: [support.ja.md](./support.ja.md)

## About the trial

A free 7-day trial of GrooveSeekDesktop (the App) is available. All features can be used during the trial period. After the trial period ends, a purchase is required. The index you create is saved on your PC and can still be used as-is after purchase.

## If "The trial period has ended" appears after purchase

The license information on the Microsoft Store side may still be out of date. Please try the following in order.

- Check that you are signed in to the Microsoft Store with the Microsoft account used for the purchase
- Sign out of the Microsoft Store, restart the PC, and then sign in again
- In Windows "Settings" → "Apps" → "Installed apps", run "Repair" for the App, and if that does not fix it, run "Reset"
- If it is still not fixed, uninstall the App once and reinstall it from the Microsoft Store

The index you created can still be used as-is after purchase, but "Reset" and reinstalling delete the index and settings, and they are rebuilt the next time the App starts.

## If some documents are not indexed

The following documents and folders are not indexed. They do not appear in search results or in the document list shown before a search.

- A document larger than 50 MB (Word, Excel, PowerPoint, PDF, Markdown or text alike)
- Anything inside a folder whose name starts with `.` (a period), a folder named `node_modules`, the Recycle Bin (`$RECYCLE.BIN`), or `System Volume Information`
- Anything inside a folder the App cannot read (no access permission, not yet downloaded to the PC by OneDrive or similar, a disconnected network drive, and so on)
- Password-protected PDF or Office documents

The supported formats are Word (`.docx`), Excel (`.xlsx`), PowerPoint (`.pptx`), PDF (`.pdf`), Markdown (`.md`) and text (`.txt`). The older formats (`.doc` / `.xls` / `.ppt`) are not supported.

For why the App could not read a file and what to do, by reason, see [Files that couldn’t be read](./troubleshooting.md).

## System requirements

- Windows 10 version 2004 or later, or Windows 11 (x64)
- It cannot be installed on older versions of Windows 10. Please update to version 2004 or later with Windows Update before using it
- The first model download requires an internet connection and at least about 2.3 GB of free space (the index needs additional space on top of this)

## Contact

Inquiries about the App are accepted through GitHub Issues ([https://github.com/alphabet-h/alphabet-h.github.io/issues](https://github.com/alphabet-h/alphabet-h.github.io/issues)). If you do not have a GitHub account, please use the contact information listed in the description on the App's Microsoft Store product page.

For the information the App handles, see the [privacy policy](./privacy.md).
