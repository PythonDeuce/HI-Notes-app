# HI Notes

Higher Intelligence Notes: sticky notes for the desktop that take dictation, save as files, tuck away with one key, and come back where you left them.

HI Notes began as the sticky notes of [TimePeace](https://github.com/PythonDeuce/TimePeace-app), the all in one desktop clock, and shares its wrapper (`desktop/widget.py`), its store, its settings and its windows. Since 0.2.0 it carries its own code on top: `js/notes-smart.js` (the rules that read the words), `js/notes-extras.js` (everything a note does beyond writing), `js/hub-extras.js` (the hub beyond the list), `desktop/tp_extras.py` and `desktop/tp_qr.py` (the wrapper's hands and the QR code). `scripts/derive_from_timepeace.py` is kept for the record and refuses to run over them.

## What a note can do

- **Write fast.** Markdown as you type, answers after `=` (sums, unit conversions, temperatures, a time in another zone, the sum of a column), snippets (`;key`), a timestamp on Ctrl+;, tables, outline lists, find and replace.
- **Remember for you.** A line with a time offers a reminder; `due Friday` sets a due date; timers, snoozes, checklists that reset, a journal with a heading per day, a daily brief on the hub and at a set time.
- **Read the words.** Title and tag suggestions, Ask your notes in the hub, Summarize and Tidy (a local model such as Ollama when one is set, built in rules otherwise), text from pictures and handwriting through the system's reader.
- **Stay where they belong.** Zones, stacks, roll up, focus view, follow a program's window, a hotkey per note, the virtual desktop they were on, gather and put back.
- **Keep secrets and history.** Private notes encrypted with a password; every save kept with a slider to restore.
- **Reach out.** A phone page on your network with a QR code, notes sent between computers, a web capture bookmarklet, the clipboard catcher, type a note into the window in front, read it back aloud, voice memos with transcripts, print the wall, imports from Sticky Notes, Stickies and Google Keep, portable mode.

Every feature works on Windows, macOS and Linux; the system's own reader, voice and screen picker are used where they differ.

## Run from source

    pip install -r desktop/requirements.txt
    python desktop/widget.py

Windows can double click `HINotes.bat`. Settings live in the `HI Notes` folder under your user's application data.

## Releasing

`python scripts/release.py X.Y.Z` tags and pushes; the workflow builds Windows, macOS and Linux; `python scripts/publish.py X.Y.Z` publishes the build on `PythonDeuce/HI-Notes-app`.

## License

MIT, see LICENSE.
