<p align="center">
  <img src="https://tilemaps.com/static/img/logo-dark-theme-2x.png" alt="Tilemaps.com" height="64">
</p>

<h1 align="center">Tilemaps Store for Defold</h1>

<p align="center">
  Import <a href="https://tilemaps.com">Tilemaps.com</a> projects into <a href="https://defold.com">Defold</a>.
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License: MIT"></a>
  <img src="https://img.shields.io/badge/Defold-editor%20script-1a1a2e?logo=defold&logoColor=white" alt="Defold editor script">
  <img src="https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-blue.svg" alt="Platform">
  <a href="https://tilemaps.com"><img src="https://img.shields.io/badge/marketplace-tilemaps.com-ff5555.svg" alt="Tilemaps.com"></a>
</p>

## Installation

This is a Defold editor script, so it installs like any other library dependency.

1. Open your `game.project` file (in the editor, or as text).
2. Under Dependencies, add the URL of the latest release zip:

   ```
   https://github.com/EVEVGames/Tilemaps-Store-for-Defold/archive/refs/tags/1.3.zip
   ```

3. Select Project → Fetch Libraries in the Defold editor.

After the library is fetched, the store shows up in the editor's Project menu as "Tilemaps Store".

## Getting started

The first time you open it, the store asks for your Tilemaps.com API token.

Click "Open account settings" in the dialog, or head straight to
[tilemaps.com/settings/account](https://tilemaps.com/settings/account), copy your
personal token, paste it into the field and press Enter.

The token is kept in the editor's global preferences, so you only type it once. If a
saved token stops working, you'll be asked for a new one.

## Tabs

The store opens as a single dialog with five tabs:

- **Explore**: the public marketplace. Search by title and browse everything you can
  download or buy.
- **My Projects**: projects you own, including their in-progress dev builds.
- **My Collaborations**: projects you were invited to work on. Each card shows your role.
- **My Purchases**: projects you've bought.
- **Downloaded**: a local registry of what you already imported into this project. It
  remembers the folder each one went into and has an Update button to pull the latest
  version.

Cards show a thumbnail, how much content the project has (tilemaps, tilesets, assets) and
a version selector. Downloading extracts the project's Defold export into a folder you
pick, and you can choose whether to include project assets and whether to overwrite
existing files.

## Development build vs. releases

The version selector offers up to two kinds of versions:

**Development build** is the live, work-in-progress build. It always reflects the current
state of the project on Tilemaps.com, so it can change at any time. You'll see it for
projects you own and for projects you collaborate on, and it's preselected when available.

**Releases** are published snapshots (Release #1, Release #2, and so on), with the most
recent marked as latest. They never change once published, which usually makes them the
safer thing to ship with.

### Updating an imported project

1. Open Tilemaps Store from the Project menu and go to the Downloaded tab.
2. Find the project. The card shows the folder it was imported into.
3. Pick the version you want: a newer release, or the latest development build if the
   project is yours or you collaborate on it.
4. Press Update. The files are re-downloaded into the same folder as before.

Leave Overwrite enabled when updating, otherwise the old files stay. If you edited
anything inside the imported folder, back it up first, since matching files are replaced.

## License

MIT, see [LICENSE](LICENSE). © 2026 Tilemaps.com
