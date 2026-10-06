# Mishima Color Editor 1.1.0

Live color editor for the electrics of **TEKKEN 8**.
Supported characters: **Kazuya, Jin, Devil Jin, Reina and Heihachi**.

Change the color of every electric (EWGF, EWHF, ETU, ETGF, EWGK, HWGF, HTGF), part by part, with a solid color or a three-color gradient, and see the result directly in game.

---

## Requirements

- Windows 10 or 11 (64-bit)
- TEKKEN 8 (PC)
- An active **MCE Access** membership on Patreon, or a key given by the author
- Nothing else to install: the app is a single file, `MCE.exe`.

---

## Getting started

1. Download **`MCE.exe`** from the latest release.
2. Put it wherever you like (Desktop, Documents, a games folder...).
3. Double-click it.
4. Unlock it once (see below).

> **Windows warning on first launch**
> The app is not signed, so Windows may block it the first time. Your browser may also ask you to confirm the download of an `.exe` file.
>
> - **Windows 10 (Microsoft Defender SmartScreen):** Windows shows *"Windows protected your PC"*. Click **More info**, then **Run anyway**.
> - **Windows 11 with Smart App Control turned on:** there is no "Run anyway" button. Unsigned apps are blocked as long as Smart App Control is on. To run the editor, turn it off in **Windows Security** > **App & browser control** > **Smart App Control settings** > **Off**.
>
>   Note: on some Windows 11 versions, Smart App Control cannot be turned back on afterwards without resetting Windows. Make this choice knowingly.
> - **Windows 11 with Smart App Control off:** same as Windows 10, click **More info** > **Run anyway**.

**Tip:** for a clean desktop icon named just "MCE", right-click `MCE.exe` > **Show more options** > **Send to** > **Desktop (create shortcut)**, then rename the shortcut to `MCE`.

---

## Unlocking MCE

After the loading screen, the unlock window appears. Nothing touches the game until MCE is unlocked.

> **Early access:** MCE will become completely free later. The paid access and the unlock system are only for the early-access period, planned to last about a month.

**With Patreon**

1. Subscribe to the **MCE Access** tier on [patreon.com/johvtsu](https://www.patreon.com/johvtsu). One month is enough.
2. In MCE, click **LOG IN WITH PATREON**. Your browser opens the official Patreon page: sign in and accept.
3. Go back to MCE: it shows **UNLOCKED** and opens the editor.

**With a key**

Click **I have a key**, type the key you were given, then **UNLOCK**.

**Good to know**

- You unlock **once per PC**. The editor then works offline and never asks again for this version.
- You can cancel your subscription afterwards: your version stays unlocked.
- **Bug-fix updates** are free and install without logging in again.
- **During early access**, big updates are part of the early-access perks: after installing one, MCE asks you to log in with Patreon again (active membership needed). The update window tells you before you install it.
- **When early access ends**, a free update removes the unlock step for everyone.
- MCE never sees your Patreon password: the login happens on Patreon's own page. The licence check only uses your Patreon membership status and an anonymous identifier of your PC.

---

## How to use

1. Start TEKKEN 8, then start the editor (or the other way round).
2. Click **MOD ON** (top of the window). The **TEKKEN 8** indicator turns green when the game is connected.
3. Pick a **character** (portraits on the side), then an **electric** (tabs at the top).
4. Pick a **part** in the list:
   - **Upper Trail** and **Lower Trail**: the two trails of the move.
   - **Electricity 1** and **Electricity 2**: the lightning effects.
5. Choose a mode for that part:
   - **NATIVE**: TEKKEN's original colors.
   - **STATIC**: one solid color (color picker, HEX or RGB).
   - **GRADIENT**: three colors A, B and C, with their distribution and HSV or RGB blending.
6. Adjust **Glow** and **Intensity** if you want a stronger effect: drag the slider, or type an exact value (0.00 to 10.00) in the field next to it and press Enter. Values below 1.00 change nothing.
7. Press **APPLY PART** (this part only) or **APPLY ELECTRIC** (all 4 parts at once).
   The colors appear the next time the electric shows up in game.

An orange mark means *edited but not applied yet*.

- **MOD OFF** puts TEKKEN's original colors back.
- **Closing the editor** also puts them back. A short "Restoring TEKKEN's colors" message shows while it happens.

### Copy and paste

- **COPY** (next to the color fields) opens a small menu:
  - **Copy this part**: the selected part (mode, colors, distribution, HSV/RGB, Glow and Intensity).
  - **Copy all parts**: the 4 parts of the electric, each with its own mode.
- **PASTE** puts what you copied into the selected part, or into the 4 parts. Nothing is applied in game until you press APPLY.
- In **Options > Copy button**, you can make COPY skip the menu and always copy the part (**PART**) or the 4 parts (**ALL**).

---

## Profiles

- Each character has **8 profiles**. Open the list with the **PROFILE** button at the bottom.
- **SAVE** stores all the electrics of the character in the selected profile.
- **LOAD** loads the profile and applies it in game.
- To **rename** a profile, hover it in the list and click the pencil.
- To **delete** a profile, go to **Options > Danger zone**.

---

## Sharing presets with friends

- **EXPORT** creates a preset file (`.json`) from the selected profile. You can export:
  - one electric,
  - several electrics,
  - or only some parts.
- **IMPORT** opens a preset file, checks it, and lets you choose what to take from it. Only the parts you pick are replaced. You can apply the import in game right away.

---

## Options (gear icon)

- **Layout**: horizontal or vertical window.
- **Backgrounds**: the background pair. It switches automatically at every launch.
- **Interface**:
  - confirmations before resets and deletions,
  - start the mod with the editor,
  - warning about unapplied edits when closing,
  - **Copy button**: PART, ASK (menu) or ALL.
- **Diagnostics**: exports a report (zip) to help solve a problem.
- **Danger zone**: reset all colors to native, delete the selected profile.

---

## Updates

At start-up the editor checks the GitHub releases for a newer version.

If you accept the update, the editor:

1. turns MOD OFF and restores TEKKEN's original colors,
2. downloads the new version and checks its SHA256 fingerprint,
3. replaces the EXE and restarts by itself.

Your settings, profiles and unlock are kept. During early access, a big update asks you to log in with Patreon once after restarting.

---

## Important

> **Disclaimer:** this tool modifies the game's memory. You use it **at your own risk**. The author accepts **no responsibility** for any ban, account restriction, data loss or other consequence resulting from its use, **including any use while playing online**. Using it online is strongly discouraged and entirely your own decision.

- **Offline modes only** (Practice, Arcade, Story...). Close the editor before playing online. TEKKEN's online protection may refuse to connect while a program edits the game's memory.
- If the editor asks you to **restart TEKKEN 8**, close the game and start it again. MOD turns back on by itself.

  This happens when an old copy of your colors could not be checked safely, so the editor refuses to touch it. It is now much rarer: the editor recognises when the game has reused the memory of an old effect for a new one.

---

## Your data

Settings, profiles, your unlock and diagnostic reports are stored in:

```
C:\Users\<your name>\AppData\Roaming\MishimaColorEditor
```

Quick access: press **Win + R**, type `%AppData%\MishimaColorEditor`, then press Enter.

**Uninstall:** delete `MCE.exe` and this folder. Nothing else is installed on your PC. (Deleting the folder also removes your unlock: you would log in again on a new install.)

---

## Checksum

GitHub shows the SHA256 fingerprint of `MCE.exe` next to the download. The editor uses it to verify every update.

---

## Credits

- Fonts: Bebas Neue and Chakra Petch, SIL Open Font License 1.1 (see `THIRD_PARTY_LICENSES.txt`).
- Fan-made tool, not affiliated with or endorsed by Bandai Namco. TEKKEN is a trademark of Bandai Namco Entertainment Inc.
