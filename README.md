# Field Book

A single-file, offline reference bank for the things you don't want to relearn twice — how to fix it, where to find it, what to check first.

No install, no server, no account. Open the file, pick a folder, start filing things away.

**[Open Field Book →](https://pilipjan.github.io/Field-book/)**

---

## What it's for

Not a wiki, not a job aid — a personal data bank. Every time you solve something worth remembering, it goes in as an entry: a title, a line of business, your notes on how you fixed it or where you found it, and a screenshot or two if that helps. Next time it comes up, search and it's there.

## How it works

- **Live folder storage** — the first time you open it, you choose a folder on your computer. Every entry becomes its own subfolder inside it.
- **Real files, not a database blob** — each entry's folder holds a plain `notes.txt` (title, category, keywords, your write-up) plus any screenshots as actual image files. Open the folder in Explorer or Finder and it all just reads like notes you left yourself.
- **Search and filter** — by keyword, category (line of business), or extra tags like a city or insured name.
- **Nothing leaves your computer.** No upload, no account, no tracking. The app only talks to the folder you pick.

## Using it

1. Open `index.html` in **Chrome or Edge** (this needs the File System Access API — Safari and Firefox aren't supported yet).
2. Choose or create a folder — this becomes your Field Book.
3. Add an entry: title, line of business, notes, and any screenshots (click, drag-and-drop, or paste straight from your clipboard).
4. Come back anytime — the browser will ask you to reconfirm access to the folder once per session, then you're back in.

## Folder structure

```
Your Chosen Folder/
├── index.json                     ← lightweight index the app reads for search/listing
├── reset-office-printer-ip-abc123/
│   ├── notes.txt
│   └── screenshot-1.png
└── hazard-code-supplemental-def456/
    ├── notes.txt
    ├── screenshot-1.png
    └── screenshot-2.png
```

`index.json` is just for speed — the real record is the folder itself, so it's still useful even if you never open the app again.

## Notes

- A folder's name is set when the entry is first created and doesn't change if you edit the title later — the `notes.txt` inside always reflects the latest title.
- Works fully offline once loaded; the "live" part only means it can read and write real files instead of browser storage.
