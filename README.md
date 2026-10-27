# 🌌 Sol’s RNG Tracker

A Windows companion app for keeping track of your **Cyberspace, Dreamspace, and Glitched** sessions in Sol’s RNG.

Record your rolls, potions, and aura drops, view your session history, and keep your progress saved between launches.

## 📥 Download

### [Download the latest release](https://github.com/zaharagiualexandru/SolsRNGTracker/releases/latest)

1. Open the latest release and expand **Assets**.
2. Download **SolsRNGTracker-v1.0.0-win-x64.zip**.
3. Right-click the ZIP and select **Extract All**.
4. Open **AppFiles** and run **CyberspaceTracker.exe**.

The download includes the .NET runtime. **You do not need Visual Studio or a separate .NET installation to use it.**

For shortcut instructions, read the **README.txt** included in the download. Keep the EXE and its supporting files together inside **AppFiles**.

**Platform:** 64-bit Windows.

> Download the attached app ZIP to use the tracker. GitHub’s “Source code” downloads contain the editable project.

## ✨ Features

### 🌌 Cyberspace

- Record rolls for each Cyberspace session.
- Track Warp potions, Tidal Wave Shifters, and PLC Device usage.
- Record **Meta** and **illusionary** drops.
- View total rolls, aura totals, and session history.
- See cumulative illusionary probability based on recorded rolls.
- Animated dark-blue visuals inspired by illusionary.

### 🌸 Dreamspace

- Track potion usage for each Dreamspace session.
- Record **Borealis** and **Dreammetric** drops.
- Pink-themed visuals with animated white and pink waves.

### ⚡ Glitched

- Track potion usage for each Glitched session.
- Record **Glitch** and **Oppression** drops.
- Animated symbols, flickering aura effects, and periodic background glitch effects.

### 🧪 Potion Tracking

Dreamspace and Glitched support:

- **Oblivion**
- **Godlike**
- **Heavenly**
- **Potion of Bound**
- **Tear of the Goddess**

### 📝 Session Management

- Add, edit, and delete sessions.
- Review previous entries and running totals.
- Automatically save changes locally.

This is a **manual tracker**. It does not automatically detect Roblox rolls, potion usage, or aura drops.

## 🎲 Understanding illusionary Probability

The tracker uses a **1 in 10,000,000** chance per eligible roll.

The displayed cumulative probability represents the chance of getting **at least one illusionary** across the recorded number of rolls:

`Probability = 100 × (1 − (1 − 1/10,000,000)^rolls)`

For example, **100,000 rolls ≈ 0.995%**.

This is a statistical estimate, not a guarantee or a pity counter. Previous unsuccessful rolls do not increase the chance of the next roll.

## 💾 Saving Your Progress

Your sessions save automatically under your Windows account:

`%LOCALAPPDATA%\CyberspaceTracker`

The tracker stores separate files for each biome:

- `cyberspace.json`
- `dreamspace.json`
- `glitched.json`

Each Windows account has its own progress. Saves are stored separately from the app’s installation folder.

To back up your progress, close the tracker and copy the entire save folder somewhere safe.

## 🔄 Updating the App

1. Close the tracker.
2. Back up `%LOCALAPPDATA%\CyberspaceTracker`.
3. Download and extract the new release into a new folder.
4. Launch the new version.
5. Confirm your existing sessions appear.

**Keep your AppData save folder.** New compatible versions read the existing saves from that location. Check each release’s notes for any additional update instructions.

If your shortcut still points to the old app folder, create a new shortcut.

## 🚧 Planned Updates

Planned for the next update:

- 🌌 **Singularity** — a dedicated biome tracking tab.
- 🌲 **Radiant Forest** — a dedicated biome tracking tab.

These tabs are **not included in v1.0.0**.

## 🛠️ Built With

- **C#**
- **WPF**
- **.NET 10**
- **JSON** for local save data

## 💻 Running From Source

To edit or build the tracker, use Windows with the **.NET 10 SDK** and a compatible Visual Studio installation with the **.NET desktop development** workload.

1. Clone or download this repository.
2. Open **CyberspaceTracker.slnx** in Visual Studio.
3. Build and run the project.

Running from source uses the same save location as the released app. Back up your saves before testing changes and close other copies of the tracker.

## 🤝 Feedback & Contributions

Bug reports, suggestions, and contributions are welcome.

- Open an **Issue** to report a problem or suggest a feature.
- Include reproduction steps and screenshots when reporting bugs.
- Fork the repository and submit a **Pull Request** to propose code changes.
- Preserve compatibility with existing saves when changing data storage.

## 📄 License

Licensed under the **MIT License**. See [LICENSE](LICENSE) for details.

---

*Unofficial fan-made companion app. Not affiliated with or endorsed by Roblox or the creators of Sol’s RNG.*
