---
title: "d2xl cIOS for Wii mini (experimental)"
---

{% include toc title="목차" %}

If you need help with anything regarding this tutorial, please join [the Wii mini Hacking Discord server](https://discord.gg/6ryxnkS) (recommended)
{: .notice--info}

While [cIOS](https://wiibrew.org/wiki/Custom_IOS) has largely been supplanted by AHBPROT, which gives complete hardware access, it still has useful applications. For example, this enables the functionality of USB loaders like USB Loader GX and WiiFlow, alongside other pieces of homebrew like SaveGame Manager GX. You can skip this process if you want, but generally it extends your Wii with little to no downsides.

This guide is only intended for Wii mini users. If you have a Wii, follow [this guide](cios) instead.
{: .notice--warning}

Do not attempt to install a Wii IOS or System Menu on the Wii mini. Doing so will likely [brick](bricks#ios-brick) your console.
{: .notice--warning}

This d2x cIOS installer was originally developed for the Wii U's vWii by DaveBaol and custom cIOS was created by Leseratte for the Wii mini. The original download page can be found [here](https://wii.leseratte10.de/d2xl-cIOS/). Leseratte's GitHub page can be found [here](https://github.com/Leseratte10/d2xl-cios). Please note that this cIOS is still experimental, though no problem with functionality has been reported.
{: .notice--info}

### 준비물

* A Wii mini with the Homebrew Channel installed
* A USB drive
* Leseratte's [d2xl cIOS Installer](/assets/files/d2xl_wii_mini_cIOS_installer_v1_beta2.zip)

### 진행 방법

#### Section I - Downloading

1. 콘솔의 전원을 꺼 주세요.
1. Insert your USB drive into your computer.
1. Create a folder named `apps` on the root of your USB drive if it does not already exist.
1. Copy the `d2x-cios-installer` folder from the d2xl cIOS Installer `.zip` to the `apps` folder on your USB drive.
1. Reinsert your USB drive into your console.
1. 콘솔의 전원을 켜 주세요.
1. Homebrew Channel을 실행해 주세요.
1. Launch d2xl cIOS Installer from the list of homebrew.

#### Section II - Installing

1. Select `Continue`.
1. Set the options to the following:
    ```
    Select cIOS <d2xl-v1-beta2>
    Select cIOS base <57>
    Select cIOS slot <249>
    ```
    + Take a note of the version number under notes (`IOS57-64-` ending in either `v31776` or `v31775`)
1. Press A to install.
    + If the install fails with a `TMD version mismatch` error, press left or right on the +Control Pad over the `Select cIOS base` option until the version number is different than the one you tried before. The number 57 will not change.
1. When the process is complete, exit the installer.

[Continue to making a NAND Backup using RealWnd](wnd-mini)
{: .notice--info}

#### Enabling Ethernet

If you wish to use Wiimmfi with Ethernet on a Wii mini, you have to run the [Ethernet Enabler Homebrew](/assets/files/Wii_Mini_Ethernet_Enable.zip) app made by Fullmetal5. To run it, just unzip it in the `apps` folder of your USB drive and run it from the Homebrew Channel.

The Wii and Wii mini consoles are only known to work with Ethernet adapters using the AX88772 chip. Please check that the product is compatible before you buy. This one from UGREEN is known to be compatible: [Amazon Europe](https://www.amazon.de/dp/B00MYT481C), [Amazon US](https://a.co/d/3OcSJDS)
{: .notice--info}

[여기를 눌러 사이트 탐색으로 돌아갑니다.](site-navigation)
{: .notice--info}
