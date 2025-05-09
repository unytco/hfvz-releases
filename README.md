# Domino Releases
![GitHub release (latest by date)](https://img.shields.io/github/v/release/unytco/domino-releases?style=for-the-badge)
![GitHub All Releases](https://img.shields.io/github/downloads/unytco/domino-releases/total?style=for-the-badge)


## Related docs
- [Test Plan](./testing_docs/1_0_testing_plan.md)
- [Phase 2 Testing Details](./testing_docs/2_0_phase_2_testing_details.md)
- [How to install Domino app?](./README.md#installation)
- [Intro to RAVEs (Three Layers)](./testing_docs/1_2_three_layers_of_raves.md)
- [RAVE Library](https://github.com/unytco/rave_library)
- [Feedback Board](https://github.com/orgs/unytco/projects/5/views/1)

## Intro
Domino is a Holochain based application for creating agent-centric, peer-to-peer, Mutual Credit accounting systems with smart contract like functionality.

We are working with potential partner projects like yours as we build out this software to ensure that it meets the needs of your team as well as your community of users.

## Overview
This [Test Plan](./testing_docs/1_0_testing_plan.md) document gives a bit of a overview of the sorts of UX / UI feedback that we are seeking at present.

## Installation

Download the appropriate version for your system.



| Releases    | 
| --------    | 
|    [macOS x84 (intel)](https://github.com/unytco/domino-releases/releases/download/v0.10.0/co.unyt.domino-0.10.0-x64.dmg)  |
|    [macOS arm64 (silicon)](https://github.com/unytco/domino-releases/releases/download/v0.10.0/co.unyt.domino-0.10.0-arm64.dmg)    |
|    [Linux Debian](https://github.com/unytco/domino-releases/releases/download/v0.10.0/co.unyt.domino_0.10.0_amd64.deb)  (recomended)  | 
|    [Linux AppImage](https://github.com/unytco/domino-releases/releases/download/v0.10.0/co.unyt.domino-0.10.0.AppImage)   (read note below) | 
|    [Windows](https://github.com/unytco/domino-releases/releases/download/v0.10.0/co.unyt.domino-0.10.0-setup.exe)    | 
|    [Android]() (no release available)    |
|    [iOS]() (no release available)    |


> [!IMPORTANT]
> If you encounter sandbox-related issues, you can try running the AppImage with:
> ```bash
> ELECTRON_DISABLE_SANDBOX=1 ./domino.AppImage
> ```
> This is automatically configured in the latest version, but might be needed for manual execution in some cases.


All available versions can be found in the [Releases](
https://github.com/unytco/domino-releases/releases)

Once installed, set up Domino either with a password or without a password. In either case, the software will run locally on your device and your password will not leave your device. 

NOTE: If you set up with a password and later lose your password, we will NOT be able to help you regain access to your account. You will need to delete the software and reinstall to create a fresh account to continue testing. See below section on **Starting Fresh**.

## Setup
Note: The release for your operating system may not be code signed yet, so you may need to right click to open the file.

When you open Domino on your operating system for the first time, it will create a set of public and private keys for you that you can use to interact with others. These are stored in a private keystore (Lair) on your own machine and are used during future uses. 

To get started, you will want to install the software on a couple of devices so you can try sending, executing, and receiving transactions. 

## Starting Fresh
Details on removal and reinstallation.

If you want to start fresh (whether because you lost a password or for another reason), uninstall the old version and then reinstall again. On Mac, you will also need to delete your local data:

Here are the steps for Uninstalling, Deleting Local Data and Reinstalling the app:

1. Close the app. 

2. Delete the domino file from your applications folder. 

3. Open the Terminal application
4. In Terminal, type the following two commands and hit enter after each:

```
cd ~/Library/Application\ Support
```

```
rm -rf co.unyt.domino
```

That co.unyt.domino file had your local data in it. 

Now that it is deleted, you can again install domino and start fresh with a new account.

Next, dive into the [Test Plan](./testing_docs/1_0_testing_plan.md).


## License

[![License: CAL 1.0](https://img.shields.io/badge/License-CAL%201.0-blue.svg)](https://github.com/holochain/cryptographic-autonomy-license)

Copyright (C) 2024 - 2025, unyt.co

