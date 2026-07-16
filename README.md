<p align="center">
  <img src="https://tilemaps.com/static/img/logo-dark-theme-2x.png" alt="Tilemaps.com" height="64">
</p>

<h1 align="center"><strong>Tilemaps Store</strong> for <strong>Defold</strong></h1>

<p align="center">
  Import <a href="https://tilemaps.com">Tilemaps.com</a> projects into <a href="https://defold.com">Defold</a>.
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-green.svg" alt="License: MIT"></a>
  <img src="https://img.shields.io/badge/Defold-editor%20script-1a1a2e?logo=defold&logoColor=white" alt="Defold editor script">
  <img src="https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-blue.svg" alt="Platform">
  <a href="https://tilemaps.com"><img src="https://img.shields.io/badge/marketplace-tilemaps.com-ff5555.svg" alt="Tilemaps.com"></a>
</p>

---

## Installation

Tilemaps Store is a Defold **editor script** and installs like any other Defold library dependency.

1. Open your `game.project` file (in the editor, or as text).
2. Under the **Dependencies** section, add the URL of the latest release `.zip`:

   ```
    https://github.com/EVEVGames/Tilemaps-Store-for-Defold/archive/refs/tags/1.0.zip
   ```

3. Select **Project → Fetch Libraries** in the Defold editor.

Once the library is fetched, open the store from the editor's **Project** menu → **Tilemaps Store**.

## Getting started

The first time you open **Tilemaps Store**, it asks for your **Tilemaps.com API token**.

- Click **Open account settings** in the dialog (or go to [tilemaps.com/settings/account](https://tilemaps.com/settings/account)).
- Copy your personal API token, paste it into the field, and press **Enter**.

Your token is stored securely in the editor's global preferences, so you only enter it once. If a saved token ever stops working, the store re-prompts you for a new one.

## Tabs

Once connected, the store opens as a single dialog with five tabs:

| Tab | What it shows |
| --- | --- |
| **Explore** | The public Tilemaps.com marketplace. Search by title and browse everything available to download or buy. |
| **My Projects** | Projects you own, including your in-progress **dev** builds. |
| **My Collaborations** | Projects you've been invited to work on, with your role shown on each card. |
| **My Purchases** | Projects you've bought — ready to download into any game. |
| **Downloaded** | A local registry of what you've already imported into *this* project. Shows which folder each one lives in and offers an **Update** button to re-download the latest version. |

Every card shows a thumbnail, a content summary (tilemaps · tilesets · assets), and a version selector. Downloading extracts the project's Defold export into a folder of your choosing, with options to **include project assets** and to **overwrite** existing files.

## Development build vs. Releases

Each project's version selector offers up to two kinds of versions:

- **Development build** — the project's live, work-in-progress build. It always reflects the *current* state of the project on Tilemaps.com and can change at any time. This option appears for projects **you own** (in **My Projects**) as well as projects **you collaborate on** (in **My Collaborations**), and is the default selection when available.
- **Releases** — immutable, published snapshots (`Release #1`, `Release #2`, …). The most recent one is marked **(latest)**. Releases never change once published, so they're what you'll typically ship with.

### Updating an imported project

1. Open **Tilemaps Store** from the **Project** menu and go to the **Downloaded** tab.
2. Find the project — it shows the folder it was imported into.
3. Pick the version you want from the selector (a newer **Release**, or the latest **Development build** for projects you own or collaborate on).
4. Press **Update**. The store re-downloads that version into the same folder it remembered.

> Keep **Overwrite** enabled when updating so the new files replace the old ones. If you've made local edits inside the imported folder, back them up first — overwriting replaces matching files.

## License

Released under the [MIT License](LICENSE). © 2026 Tilemaps.com
