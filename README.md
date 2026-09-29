# HI Notes

Higher Intelligence Notes: sticky notes for the desktop that take dictation, save as files, tuck away with one key, and come back where you left them.

HI Notes is built from the same code as [TimePeace](https://github.com/PythonDeuce/TimePeace-app), the all in one desktop clock, and shares its wrapper (`desktop/widget.py`), its store, its settings and its windows. `scripts/derive_from_timepeace.py` rebuilds this folder from a TimePeace checkout; the product's own pieces are its name, icon, settings folder, repositories and the hub page the main window opens (`index.html?widget=1&tool=hub`).

## Run from source

    pip install -r desktop/requirements.txt
    python desktop/widget.py

Windows can double click `HINotes.bat`. Settings live in the `HI Notes` folder under your user's application data.

## Releasing

`python scripts/release.py X.Y.Z` tags and pushes; the workflow builds Windows, macOS and Linux; `python scripts/publish.py X.Y.Z` publishes the build on `PythonDeuce/HI-Notes-app`.

## License

MIT, see LICENSE.
