# GrooveSeekDesktop: Files that couldn’t be read

> **日本語版**: [troubleshooting.ja.md](./troubleshooting.ja.md)

The “Files that couldn’t be read” list is new in v1.3 (earlier versions don’t have it).

## About this page

GrooveSeekDesktop reads the contents of the files in the folder you chose, to prepare for searching (indexing). Files it couldn’t read appear in the “Files that couldn’t be read” list with a reason. The code next to the reason (for example `encrypted`) names the reason, and matches the section names on this page.

When you contact us, please include what “Copy list” copies.

### When searches still find an earlier version {#kept_old}

If a file that was read before couldn’t be read this time, searches still find the earlier version. The row says “(searches still find the earlier version)”.

## Causes and what to do, by reason

### The file is too large {#too_large}

**Cause**: Reading a large file uses a lot of memory, so the app only reads files up to a set size (50 MB).

**What to do**: Split it into smaller files.

### Its contents are too large, counting the text taken out {#over_extraction_limit}

**Cause**: Word, Excel and PowerPoint files store their contents compressed. Unpacked, they went over the limit (text taken out of PDF and Excel files counts too).

**What to do**: Save it as several smaller files.

### Too large for this kind of file {#over_parser_limit}

**Cause**: This kind of file has a size limit for reading.

**What to do**: Split it into smaller files.

### Taking the text out took too long {#extraction_timed_out}

**Cause**: Taking the text out of a PDF or Excel file didn’t finish within the time allowed (120 seconds). Very large or complex files cause this.

**What to do**: Split it into smaller files. If you don’t need it, move it out of the folder so it no longer takes time each time files are read.

### It is password-protected {#encrypted}

**Cause**: The contents of a password-protected file can’t be read.

**What to do**: Open it in its app, remove the password and save it again. If you want to keep the password, you can leave it.

### The file is damaged or in a format this app can’t read {#corrupt_or_unsupported}

**Cause**: The file is cut short, in an old format (.doc, .xls, .ppt and so on), or its extension (the end of its name, such as “.docx”) doesn’t match its contents.

**What to do**: Open it in its app and save it again (save old .doc, .xls, .ppt files as .docx, .xlsx, .pptx). If it won’t open, the file is damaged; restore it from a backup.

### The text isn’t saved in the UTF-8 character format {#not_utf8}

**Cause**: Text files (.txt, .md) are read only when saved in the UTF-8 character format (encoding). Files made with older apps may use Shift_JIS.

**What to do**: Open it in Notepad, choose File > Save as, set the character format (Encoding) to UTF-8 and save.

### The PDF’s text comes out garbled {#text_undecodable}

**Cause**: The PDF lacks the information needed to read its characters as text (it depends on how fonts were embedded).

**What to do**: Make the PDF again from the original document (Word and so on). If there is no original, run text recognition (OCR) on it.

### The PDF has almost no text {#too_little_text}

**Cause**: A PDF of scanned paper or images holds pictures, not text.

**What to do**: Use an app or scanner feature with text recognition (OCR) to make a PDF with text.

### It has no text in it {#no_text}

**Cause**: The file has no text.

**What to do**: Add some text. If it is meant to be empty, you can leave it.

### The file couldn’t be read {#unreadable}

**Cause**: Another app has it open, you don’t have permission, or it was moved or deleted before it could be read (the reason in the list says which).

**What to do**: If another app has it open, close it in that app, then choose File > Reindex. Without permission, allow reading under Properties > Security, or ask its owner. If you moved or deleted it, you can leave this. If it keeps happening, copy the file again.

### It couldn’t be converted for searching {#embed_rejected}

**Cause**: The step that converts contents into a searchable form didn’t accept this file.

**What to do**: Splitting it into smaller files may help. If it keeps happening, contact us with what “Copy list” copies.

### The file changed while it was being read {#changed_during_read}

**Cause**: Another app changed the file while it was being read.

**What to do**: Nothing to do. It will be read again next time.

### It isn’t a regular file {#not_plain_file}

**Cause**: It is a link to somewhere else (a symbolic link, not a shortcut) or a special kind of file.

**What to do**: Put the original file the link points to in the folder.

### The same file also has another name (a hard link) {#hard_link}

**Cause**: One file has two or more names. The app can’t tell whether the other name is outside the folder you chose. So that files outside the folder (including ones you aren’t allowed to read) don’t end up in search without your knowing, it isn’t read, to be safe.

**What to do**: Copy it so each name is a separate file.

### Its name can’t be used {#unspellable_name}

**Cause**: The name of the file or folder is in a form Windows can’t handle (ending in `.` or a space, containing `:` or one of `<` `>` `"` `|` `?` `*`, or names like CON or NUL), or it is garbled and can’t be read. For a folder, the files in it can’t be read either.

**What to do**: Rename it. If File Explorer can’t rename it, use the app that named it (another OS or a sync app).

### Other reasons

**Cause**: This version of the app doesn’t know the reason.

**What to do**: Updating the app may show the reason.
