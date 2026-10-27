# emusen-themes

Themes for [EmuSen](https://github.com/RedQuE3n/EmuSen)'s big picture mode, every theme credited to its authors and kept
under its own licence.

Big picture reads ES-DE's theme format, so the themes here are ES-DE themes: ones made for EmuSen, and links to the
others in their authors' own repositories. None is bundled with the program.

## Layout

- `themes.json`: the index EmuSen's theme downloader reads. Each entry names the theme, its author, its repository, the
  branch and **the exact commit EmuSen offers**, its licence and where that was read, ES-DE's list fields (variants,
  colour schemes, aspect ratios, …), and links to its screenshots. `emusen` holds EmuSen's own verdict on the theme once
  it has been surveyed with EmuSen's loader, and is `null` until then.
- `upstream/<theme>/`: each theme as a git submodule, a link to its authors' repository at that commit. Nothing of a
  theme is copied here; it is downloaded from its authors. `git submodule update --init upstream/<theme>` fetches one.
- `themes/<theme>/`: a theme made for EmuSen, kept here in full with its own `LICENSE`.
- `ATTRIBUTION.md` lists every theme, its authors, its licence, and the commit linked.

The themes were first gathered from ES-DE's theme list (`gitlab.com/es-de/themes/themes-list`), whose `themes.json` this
index follows; the screenshots stay in that list's repository and are linked, not copied. Moving a theme to a newer
commit is a change to its submodule and its entry, made once the new commit has been checked.

## Licences

**Each theme is under its own licence**, in its folder, and that licence governs it alone. Many ES-DE themes are under
Creative Commons licences with a NonCommercial term (Art Book Next is CC BY-NC-SA 4.0): they are shared here unchanged,
with attribution, for non-commercial use, and are never relicensed. The collection's own files (this README, the
attribution list, any index or tool) are under the GNU General Public License, version 3 (`LICENSE`).
