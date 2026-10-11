# Playbook

**A free live overlay for HoneyPlayBox / Vibe Connect streamers.** Made by Bizbon_AD.

Playbook turns your Vibe Connect activity into a clean OBS overlay. It runs entirely on your own PC. Nothing is sent anywhere.

### ⬇️ [Download the latest version](https://github.com/papagenb/PlayBook/releases/latest)

---

## What it shows

- Every tip as it comes in (who, how much, how long)
- Your tip menu, with the tier that was just hit lighting up
- Your Control Link rules
- Top tippers
- The love meter
- The Control Link QR code, shown and hidden exactly when Vibe Connect does
- Viewer joins and a live connection light
- The HoneyPlayBox logo, in the spot you choose

**Use Lovense too (or instead)?** Turn it on in Playbook and the overlay also shows your Lovense tip menu and special commands, tips, connected toys, a live Control Link panel, top tippers and the Vibe with Me QR code. Panels stay hidden until something sends them data, so the overlay fits whichever you use.

Use the built-in design as-is, or build your own with a single HTML file (full guide included).

## What you need

- Windows 10 or 11
- The Vibe Connect app, installed and signed in
- OBS (or any streaming app with a **Browser Source**)
- For Lovense (optional): the Lovense OBS Toolset in OBS, and the Lovense Cam Extension running in Chrome

## Install

1. Download `Playbook-vX.X.X.zip` from the [latest release](https://github.com/papagenb/PlayBook/releases/latest) and unzip it.
2. Put `Playbook.exe` anywhere you like (your Desktop is fine) and double-click it. Nothing to install.
3. Follow the 4 setup steps in the Playbook window (about 2 minutes, one time only).
4. In OBS, add a **Browser** source with the address Playbook gives you (`http://localhost:4336/playbook/`), size **1920 × 1080**.

Full instructions are in **READ ME FIRST - Playbook.txt** inside the zip.

> **"Windows protected your PC"?** The first time you run it, Windows may warn about an unknown publisher. This is normal for small free apps that aren't code-signed. Click **More info** → **Run anyway**.

## Privacy & safety

- **Runs only on your PC.** The overlay listens on `localhost` only. Nobody on the internet can connect to it.
- **Never sees your login.** Playbook never sees or saves your Vibe Connect login.
- **Read-only with Lovense.** It never controls your toy or changes your Lovense settings.
- **Control Link QR:** whoever scans it can control your toy while the link is active. Playbook only shows it when Vibe Connect does.
- Only use this overlay in scenes for adult platforms.

## Verify your download

Each release lists SHA-256 checksums. To check yours, open PowerShell in the download folder and run:

```powershell
Get-FileHash .\Playbook-v0.4.0.zip -Algorithm SHA256
```

The result should match the checksum on the release page.

**Virus scan:** [VirusTotal results for v0.4.0](https://www.virustotal.com/gui/file/e0c3f025f1e9f4259e13e5460d7ce8ae62e1b084476628a75277fbc36fdad52a)

## Uninstall

Quit Playbook from the tray (right-click the icon → **Quit**), then delete `Playbook.exe`.
Your settings and log are in `%APPDATA%\Playbook`. Delete that folder too to remove everything.

## Help

Found a bug or have a question? [Open an issue](https://github.com/papagenb/PlayBook/issues). Click **Open log folder** at the bottom of Playbook and attach `playbook.log`. It helps a lot.

---

Playbook is free. Made by Bizbon_AD for the community. Enjoy!

Free to use, not to resell or re-upload. See [LICENSE](LICENSE).
