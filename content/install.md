+++
date = '2026-05-29'
draft = false
title = 'Install'
description = 'How to install the Golden Forgery expansion for Umineko Golden Fantasia.'
+++

{{< alertBlockquote type="warning" >}}
**Sample content — replace before launch.** The steps below are placeholders and almost certainly wrong; edit this page (`content/install.md`) with the real instructions.
{{< /alertBlockquote >}}

## Requirements

Before you start, make sure you have:

- A legitimate copy of *Umineko Golden Fantasia* (version **X.Y.Z** or later).
- **Windows 10 / 11** (other OSes may work via Wine — untested).
- At least **TBD MB** of free disk space.
- The latest **DirectX runtime** installed.

## Download

Grab the latest release of Golden Forgery from the releases page:

- **[Download Golden Forgery vX.Y.Z](#)** *(replace with the real link)*
- Mirror: **[GitHub Releases](#)** *(optional)*

Verify the download against the checksum on the releases page before continuing.

## Install steps

1. **Back up your game folder.** Copy your `Umineko Golden Fantasia/` directory somewhere safe so you can roll back if anything goes wrong.
2. **Extract the archive.** Unzip `golden-forgery-X.Y.Z.zip` into a temporary folder.
3. **Copy files into the game directory.** Move the contents of the extracted `data/` folder into your `Umineko Golden Fantasia/` install directory, overwriting when prompted.
4. **Run the patcher** (if included). Double-click `forgery-patch.exe` and follow the prompts.
5. **Launch the game** as you normally would. You should see the *Golden Forgery* logo on the title screen.

## Verifying the install

If everything worked, the title screen will show "**Golden Forgery vX.Y.Z**" in the corner. New characters and stages will appear in their respective select screens.

## Troubleshooting

**The game crashes on launch.**
TBD — usually a missing dependency or a leftover file from a previous mod. Try a clean install over a vanilla copy of the game.

**My save files are gone.**
Saves live in `%APPDATA%/UminekoGoldenFantasia/` and are not touched by the install — restart the game once and they should reappear. If they don't, restore from the backup you made in step 1.

**Multiplayer doesn't match.**
Both players must be on the exact same Golden Forgery version. Check the version string on the title screen.

For anything else, see the **[News](/)** page for the latest known issues, or reach out via *(insert your support channel here — Discord, issue tracker, etc.)*.

## Uninstall

To go back to vanilla, delete your modded `Umineko Golden Fantasia/` directory and restore the backup you made in step 1. Saves are preserved.
