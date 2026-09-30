# GrooveSeekDesktop

> **日本語版**: [index.ja.md](./index.ja.md)

On first launch, GrooveSeekDesktop downloads the model used for search (about 2.3 GB) from Hugging Face. The download requires an internet connection and free disk space. The download happens only the first time (it is downloaded again if it stops partway, or if a downloaded model can no longer be read).

GrooveSeekDesktop (the App) is an app that finds documents in your folders by the words you type.

## What it does

- Reads Word, Excel, PowerPoint, PDF, and Markdown documents in the folders you choose, and builds an index
- When you enter the words you are looking for, it lists documents with similar content and the passages that matched. You can find documents even if you do not remember the file name
- Documents you find can be opened directly in your usual apps. It can also show where the file is located

## Your documents never leave your PC

- The index is kept only inside this PC. Neither the contents of documents nor search terms are sent outside the PC
- The App connects to the internet only when it downloads the model used for search (normally only the first time)

## The AI only searches

- The App uses an AI model for search, but the AI never writes or summarizes text. What it shows is only your own documents and the relevant passages in them

## System requirements

- Windows 10 version 2004 or later, or Windows 11 (x64)
- It cannot be installed on older versions of Windows 10. Please update to version 2004 or later with Windows Update before using it
- The first model download requires an internet connection and at least about 2.3 GB of free space (the index needs additional space on top of this)

## How to get it

GrooveSeekDesktop is distributed through the Microsoft Store.

## Related pages

- [Support](./support.md)
- [Privacy policy](./privacy.md)
