# Aowu Modding Toolkit

A two-part toolkit by **Aowu (嗷呜)** for the *SecretFlasherManaka* modding scene:

| Tool | What it does |
| --- | --- |
| **Aowu MOD Manager** | Desktop app for players — browse, install, update, and manage MODs. |
| **BE Resource Pack Builder** | Desktop app for creators — bundle MODs into shareable resource packs. |

Both are Windows desktop apps (PyQt5). Interface available in **English and Chinese**
(switch language from the toolbar / settings; restart to apply).

- Website & MOD market: **https://www.aowu-miao.com**
- Upcoming title: **Endless Depravity 2**

---

## Contents of this release

| File | Description |
| --- | --- |
| `嗷呜管理器-2.2.1.exe` | Aowu MOD Manager v2.2.1 (installer / portable exe) |
| `dist.rar` | BE Resource Pack Builder (packaged app) |

Both are standalone Windows executables — no Python install required.

---

## Aowu MOD Manager

The player-facing app. It connects to the online MOD market at
**https://www.aowu-miao.com** so you can find content, then handles installing and
keeping it up to date locally.

### Getting started

1. Place `嗷呜管理器-2.2.1.exe` in your **game root folder** and run it.
2. Sign in (or use **guest mode** to browse without an account).
3. Set your language from **Settings** if you prefer English.

### What you can do

- **Browse the MOD market** — search and filter community MODs pulled from the server.
- **One-click install / update** — downloads are delivered as `.mp4` resource packs;
  the manager unpacks and installs them into the game for you.
- **Import local packs** — drag `.mp4` resource packs onto the window (multi-file
  supported); the manager auto-unpacks and resolves file conflicts (overwrite / skip,
  with "apply to all" memory).
- **Manage installed MODs** — enable, disable, or fully remove a MOD (removal cleans
  up its game files without touching shared plugins).
- **Account features** — user center, VIP tiers, leaderboards, and the in-app
  currency systems tied to the platform.

> The manager talks to the server over HTTPS with a JWT token. Login credentials are
> stored in the OS keyring, not in plain text.

---

## BE Resource Pack Builder

The creator-facing app. It turns one or more MOD folders into shareable resource
packs that the Manager can import.

### Workflow

1. **➕ New MOD Folder** — create a fresh MOD entry, or **📁 Scan 'Mods' Folder** to
   auto-detect existing MODs (fills in ID, name, and cover).
2. Fill in each MOD's details: **Name, Description, Version, Category, Cover Image,
   and a Unique ID.**
3. **🎨 Card Settings** — tune the auto-generated cover card (fonts, colors, preview).
4. **🖼 Generate All Cards** / **🖼 Generate Cards (This Category)** — batch-render
   cover images.
5. Pack it up:
   - **📦 Pack All Into One** — merge every MOD into a single large pack.
   - **🔪 Pack Each Separately** — output one pack per MOD.
6. **💾 Save Project** — persist your setup so you can come back to it later.

### Categories

MODs are organized into: **Costume, Custom Task, Trainer, Texture, Feature, Other.**
Use **Filter by category** to narrow the list.

### About the resource packs

Packs are wrapped inside a **playable `.mp4` file**. The video plays normally in any
player, while the Manager knows how to unwrap and install the MOD data inside. This
keeps distribution simple — a single file that's easy to share and easy for the
Manager to recognize.

---

## Language support

Both apps ship with English and Chinese. Pick your language from the toolbar
(**Language** selector) or the settings page; the change applies after a restart.

---

## Links

- 🌐 **Website / MOD market:** https://www.aowu-miao.com
- 🎮 **Upcoming title:** Endless Depravity 2

---

## Disclaimer

These are modding tools provided as-is. All MOD content is created and shared by
users; the authors of these tools are not responsible for any content distributed
with them. Users are responsible for complying with the laws of their own country
and with the terms of any content they download.
