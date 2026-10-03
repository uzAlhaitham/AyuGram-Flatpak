# AyuGram Flatpak Repository

A personal Flatpak repository for [AyuGram Desktop](https://github.com/AyuGram/AyuGramDesktop), built automatically from the official Flatpak bundles provided by [0FL01/AyuGramDesktop-flatpak](https://github.com/0FL01/AyuGramDesktop-flatpak).

## Why This Repository Exists

The original AyuGram project provides official packages for Windows, macOS, and several Linux distributions (Arch, Fedora, etc.). However, **no official Flatpak remote** was available for users who prefer Flatpak over native packages.

To improve the experience for Flatpak users, I created this repository. It repackages the official `.flatpak` bundles from [0FL01/AyuGramDesktop-flatpak](https://github.com/0FL01/AyuGramDesktop-flatpak) into a self-hosted Flatpak remote with GPG signing and automatic updates via GitHub Actions.

This is a community-driven effort to make AyuGram more accessible on Linux systems where Flatpak is the preferred installation method.

## Credits

This repository would not exist without the hard work of others. All credit for the application itself and its packaging goes to the original creators and contributors.

### Original Application
- **[AyuGram Desktop](https://github.com/AyuGram/AyuGramDesktop)** — The main application, developed by the AyuGram team.

### Flatpak Packaging
- **[0FL01/AyuGramDesktop-flatpak](https://github.com/0FL01/AyuGramDesktop-flatpak)** — The official Flatpak packaging that provides the `.flatpak` bundles used in this repository.

### Telegram Clients
- [Telegram Desktop](https://github.com/telegramdesktop/tdesktop)
- [Kotatogram](https://github.com/kotatogram/kotatogram-desktop)
- [64Gram](https://github.com/TDesktop-x64/tdesktop)
- [Forkgram](https://github.com/forkgram/tdesktop)

### Libraries Used
- [JSON for Modern C++](https://github.com/nlohmann/json)
- [SQLite](https://github.com/sqlite/sqlite)
- [sqlite_orm](https://github.com/fnc12/sqlite_orm)
- [androidx sources](https://github.com/androidx/androidx)

### Icons
- [Solar Icon Set](https://www.figma.com/community/file/1166831539721848736)

### Bots
- [TelegramDB](https://t.me/tgdatabase) for username lookup by ID

### Tools
- **[andyholmes/flatter](https://github.com/andyholmes/flatter)** — GitHub Action used during early development.

## Installation

Add the repository and install AyuGram:

```bash
flatpak remote-add --if-not-exists ayugram-repo https://uzAlhaitham.github.io/AyuGram-Flatpak/ayugram.flatpakrepo
flatpak install ayugram
