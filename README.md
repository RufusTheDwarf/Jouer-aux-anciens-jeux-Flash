<div align="center">

# 🎮 Play Old Flash Games

**A complete, modern guide to rediscover the Flash games of your childhood — without Adobe Flash Player, using Ruffle.**

[![Ruffle](https://img.shields.io/badge/Emulator-Ruffle-ff69b4?style=flat&logo=rust&logoColor=white)](#)
[![Format](https://img.shields.io/badge/Format-SWF-6B3E26?style=flat)](#)
[![Platform](https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-0078D6?style=flat&logo=linux&logoColor=white)](#)
[![License](https://img.shields.io/badge/License-MIT-lightgrey?style=flat)](#)

<br>

[![Stars](https://img.shields.io/github/stars/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash?style=flat&color=yellow)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash/stargazers)
[![Forks](https://img.shields.io/github/forks/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash?style=flat&color=blue)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash/forks)
[![Watchers](https://img.shields.io/github/watchers/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash?style=flat&color=green)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash/watchers)
[![Issues](https://img.shields.io/github/issues/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash?style=flat&color=red)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash/issues)
[![Pull Requests](https://img.shields.io/github/issues-pr/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash?style=flat&color=purple)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash/pulls)
[![Last Commit](https://img.shields.io/github/last-commit/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash?style=flat&color=orange)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash/commits/main)
[![Contributors](https://img.shields.io/github/contributors/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash?style=flat&color=informational)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash/graphs/contributors)
[![Repo Size](https://img.shields.io/github/repo-size/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash?style=flat&color=black)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash)
[![Top Language](https://img.shields.io/github/languages/top/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash?style=flat&color=pink)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash)

</div>

---

## 📖 About

Welcome to **Play Old Flash Games**! This repository lets you **play thousands of Flash games and animations** that shaped the history of the web, **without installing Adobe Flash Player** (which has been unsupported since the end of 2020).

Thanks to **Ruffle**, an open-source emulator written in Rust, you can launch your favorite `.swf` files again on Windows, macOS, and Linux.

This guide takes you from **zero**: whether you have never touched a Flash game or you are an advanced user, you will find every step, official links, technical explanations, and solutions to common problems.

---

## 🚀 Why Ruffle?

Before diving in, it is important to understand **why you should not use Adobe Flash Player anymore** and how Ruffle solves the problem.

### 1. What was Adobe Flash Player?

For almost 20 years, **Adobe Flash Player** was the essential plugin for playing animations, games, and videos on the web. Files in the `.swf` format (Shockwave Flash) packed everything: vector graphics, sounds, and **ActionScript** code.

### 2. Why does Flash no longer work?

- **Security**: Flash Player accumulated **critical vulnerabilities**. Attackers could execute arbitrary code on your machine.
- **Performance**: heavy, power-hungry, and poorly suited to mobile devices.
- **Alternatives**: HTML5, WebGL, and WebAssembly made Flash obsolete.
- **Official end of life**: Adobe stopped support on **December 31, 2020**. Browsers blocked the plugin starting January 2021.

### 3. Why is Ruffle the modern solution?

**Ruffle** is an **open-source emulator** written in **Rust**. It is **not** a wrapper around Flash Player, but a **full reimplementation** of the ActionScript virtual machine and the Flash API.

| Advantage | Detail |
|---|---|
| **Secure** | Sandboxed, no inherited vulnerabilities |
| **Open source** | Auditable code, active community |
| **Cross-platform** | Windows, macOS, Linux, browser |
| **Actively maintained** | Regular updates |
| **Free** | No cost, no ads |

> ⚠️ **Never download an "old Flash Player"** from unofficial sites. These files are often malware. Use Ruffle only.

---

## 📦 Installing Ruffle

Follow the guide for your operating system.

### 🪟 Windows

1. **Download Ruffle**: Go to the [official Releases page](https://github.com/ruffle-rs/ruffle/releases). Grab the latest stable version (for example `ruffle-nightly-YYYY_MM_DD-windows-x86_64.zip`).
2. **Extract the archive**: Right-click the `.zip` file, then **Extract All**.
3. **Place the folder**: Move the extracted folder somewhere permanent, like `C:\Ruffle\`.
4. **Launch Ruffle**: Double-click `ruffle.exe`. A window opens.
5. **Open a game**: Click **Browse**, pick a `.swf` file, and the game launches.

**Advanced alternative (winget)**:
```bash
winget install --id=Ruffle.Ruffle -e
```


### 🍎 macOS

1. **Download Ruffle**: From the [Releases page](https://github.com/ruffle-rs/ruffle/releases), pick the `macos` build (`.tar.gz` file).
2. **Extract the archive**: Double-click the `.tar.gz`, or use the Terminal:
   ```bash
   tar -xzvf ruffle-nightly-*.tar.gz
   ```
3. **Open the app**: **Right-click** `Ruffle`, then choose **Open**. (macOS shows a security warning for apps downloaded from the internet.)
4. **Allow it**: If macOS blocks the launch, go to **System Settings → Privacy & Security** and click **Open Anyway**.
5. **Launch a game**: Open Ruffle, click **Browse**, pick a `.swf`.

**Homebrew alternative**:
```bash
brew install --HEAD ruffle-rs/ruffle/ruffle
```

### 🐧 Linux

**Recommended method: Flatpak**

1. Install Flatpak if you haven't already (see [flatpak.org](https://flatpak.org/setup/)).
2. Install Ruffle:
   ```bash
   flatpak install flathub rs.ruffle.Ruffle
   ```
3. Launch Ruffle from your app menu or with:
   ```bash
   flatpak run rs.ruffle.Ruffle
   ```

**Alternative method: direct download**

1. Download the `linux-x86_64.tar.gz` file from [Releases](https://github.com/ruffle-rs/ruffle/releases).
2. Extract it:
   ```bash
   tar -xzvf ruffle-nightly-*.tar.gz
   ```
3. Make it executable:
   ```bash
   chmod +x ruffle
   ```
4. Launch:
   ```bash
   ./ruffle
   ```

---

## 📥 Official Downloads

| Tool | Required? | Purpose | Download | Documentation |
|---|---|---|---|---|
| **Ruffle Desktop** | **Yes** | Emulate Flash | [Windows](https://github.com/ruffle-rs/ruffle/releases) · [macOS](https://github.com/ruffle-rs/ruffle/releases) · [Linux](https://github.com/ruffle-rs/ruffle/releases) | [Wiki](https://github.com/ruffle-rs/ruffle/wiki) |
| **Git** | Optional | Clone the repo | [Windows](https://git-scm.com/download/win) · [macOS](https://git-scm.com/download/mac) · [Linux](https://git-scm.com/download/linux) | [Doc](https://git-scm.com/doc) |
| **7-Zip** | Recommended | Extract archives | [Windows](https://www.7-zip.org/download.html) | [Site](https://www.7-zip.org/) |
| **Flashpoint Infinity** | Optional | Library of 200,000+ games | [Download](https://flashpointarchive.org/downloads/) | [FAQ](https://flashpointarchive.org/faq) |

---

## 🎯 Where to Find Flash Games

Ruffle ships **no games**. Here are the legitimate and reliable sources for finding `.swf` files:

| Source | Content | Search | Format | Precautions |
|---|---|---|---|---|
| **Internet Archive** | Thousands of preserved Flash games | [archive.org/details/softwarelibrary_flash](https://archive.org/details/softwarelibrary_flash) | `.swf` or online emulation | Check the license of each game |
| **Flashpoint Archive** | 200,000+ games and animations | [flashpointarchive.org](https://flashpointarchive.org/) | Dedicated application | License varies by game |
| **Newgrounds** | Original games and animations | [newgrounds.com](https://www.newgrounds.com/) | `.swf` (via third-party tools) | Content is copyrighted |

> ⚠️ **Important**: A game being old **does not mean it is free of rights**. Always check the license before any redistribution.

---

## 🕹️ Launching a Game

Once Ruffle is installed and you have a `.swf` file, here is how to launch the game.

### Method 1: Drag and drop (simplest)

1. Open Ruffle.
2. Take the `.swf` file and **drag it** into the Ruffle window.
3. The game launches immediately.

### Method 2: Open from Ruffle

1. Open Ruffle.
2. Click **Browse**.
3. Select the `.swf` file in the file explorer.
4. The game launches.

### Method 3: Command line

```bash
# Windows
ruffle.exe C:\path\to\game.swf

# macOS / Linux
./ruffle /path/to/game.swf
```

---

## 📁 Recommended Organization

To avoid chaos, organize your games in dedicated folders:

```text
My_Flash_Games/
├── Ruffle/
│   └── ruffle.exe
├── Road_of_Fury/
│   ├── Road_of_Fury.swf
│   ├── assets/
│   └── info.txt
├── Alien_Hominid/
│   ├── alien_hominid.swf
│   └── ...
└── README.txt
```

- **One folder per game**: easier to manage assets (images, sounds, XML).
- **Keep all files**: do not delete side files, they are often required.
- **`info.txt`**: note the source, download date, and license.

---

## ⚠️ Troubleshooting

| Symptom | Likely cause | Check | Fix |
|---|---|---|---|
| **Black screen** | Incompatible SWF or unsupported ActionScript 3 | Test another game | Check compatibility at [ruffle.rs/compatibility](https://ruffle.rs/compatibility) |
| **Game closes** | Missing dependencies (external assets) | Inspect the game folder | Restore the missing files |
| **No sound** | Unsupported audio or missing file | Test with another game | Check audio drivers |
| **Mouse not working** | Game designed for a different input | — | Try a different version |
| **Keyboard not working** | Focus not captured by the window | Click inside the window | Restart Ruffle |
| **Multiplayer game** | Original server is gone | — | Use Flashpoint or a preservation server |

---

## 🔗 Useful Links

**Ruffle:** [Official site](https://ruffle.rs/) · [Releases](https://github.com/ruffle-rs/ruffle/releases) · [Wiki](https://github.com/ruffle-rs/ruffle/wiki) · [Compatibility](https://ruffle.rs/compatibility)  
**Flashpoint:** [Official site](https://flashpointarchive.org/) · [Download](https://flashpointarchive.org/downloads/) · [FAQ](https://flashpointarchive.org/faq)  
**Archives:** [Internet Archive](https://archive.org/details/softwarelibrary_flash) · [Newgrounds](https://www.newgrounds.com/)  
**Tools:** [Git](https://git-scm.com/downloads) · [7-Zip](https://www.7-zip.org/download.html)

---

<div align="center">

### 👤 Author

**RufusTheDwarf**

[![GitHub](https://img.shields.io/badge/GitHub-RufusTheDwarf-181717?style=flat&logo=github&logoColor=white)](https://github.com/RufusTheDwarf) [![Repository](https://img.shields.io/badge/Repo-Jouer--aux--anciens--jeux--Flash-2ea44f?style=flat&logo=git&logoColor=white)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash)

<br>

### 💖 Acknowledgements

Thanks to the open-source community, to the **Ruffle** team for their outstanding work, and to the **Flashpoint** and **Internet Archive** projects for preserving this digital heritage.

<br>

### ⭐ Show Your Support

[![Star this repo](https://img.shields.io/badge/⭐_Star_this_repo-yellow?style=flat)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash/stargazers) [![Report an issue](https://img.shields.io/badge/🐛_Report_an_issue-red?style=flat)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash/issues) [![Fork this repo](https://img.shields.io/badge/🍴_Fork_this_repo-blue?style=flat)](https://github.com/RufusTheDwarf/Jouer-aux-anciens-jeux-Flash/fork)

<br>

---

<sub>Made with ❤️ by **RufusTheDwarf** · MIT License · © 2026</sub>

<br>

*Video game heritage deserves to be preserved.* 🎮

</div>
