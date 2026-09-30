# GrooveSeekDesktop Privacy Policy

> **日本語版**: [privacy.ja.md](./privacy.ja.md)

- Publisher: koshian (こしあん)
- Applies to: the Windows app "GrooveSeekDesktop", distributed through the Microsoft Store
- Effective date: September 30, 2026

GrooveSeekDesktop (the "App") is an app that indexes and searches the documents in folders the user chooses, only inside the user's PC.
This policy explains what information the App handles and how it handles it.

## Information we collect

The App does not collect the user's information.

- The contents of the documents being indexed, file names, folder locations, and the search terms entered are not sent outside the PC.
- There is no mechanism by which the publisher (koshian) receives the user's information.

## Network communication

The App connects to the internet only when it downloads the model used for search (about 2.3 GB) from Hugging Face (`huggingface.co`) and from Hugging Face's delivery servers. It connects over IPv4.

- It downloads only in the following cases:
  - The first time the App is used
  - When a download stops because the connection failed (the App waits a little and retries automatically, making up to 5 attempts including the first)
  - The next time the App starts after it was closed in the middle of a download (the download resumes from what was already downloaded)
  - When the user presses "Retry" after the automatic retries still could not download the model
  - When a downloaded model can no longer be read (the App downloads the unreadable part again to repair it)
- During the download, these servers receive ordinary HTTPS requests. These include information that is generally delivered to the other party when communicating over the internet, such as the user's IP address.
  How Hugging Face handles this information is governed by Hugging Face's privacy policy.
- This communication never sends the contents of documents or search terms.

## What the App stores on the PC

The App stores the following only in a location dedicated to the App inside the user's PC (a private location that Windows provides for each app).

- Settings (such as the locations of the chosen folders)
- Activity records (logs)
- The document index
- The downloaded model

The user chooses which folders are indexed. All of this information stays on the user's PC; the publisher does not hold any of it. None of it is sent outside the PC. To delete it, uninstall the App. Uninstalling removes all of it.

## Telemetry (sending usage information)

The App has no mechanism (telemetry) that sends usage or error information to the publisher. It does not display ads either.

## Information collected by the Microsoft Store and Windows

Information that the Microsoft Store or Windows collects in connection with acquiring, updating, or uninstalling the App, or with the operation of Windows, is handled under Microsoft's policies, not by the App.
For details, see the Microsoft Privacy Statement.

## Changes to this policy

When this policy changes, this page will be updated and the date above will be revised.

## Contact

Inquiries about the App are accepted through GitHub Issues ([https://github.com/alphabet-h/alphabet-h.github.io/issues](https://github.com/alphabet-h/alphabet-h.github.io/issues)). If you do not have a GitHub account, please use the contact information listed in the description on the App's Microsoft Store product page.
