# YouTube Client for Fire TV and Android TV

Alternative YouTube clients for Fire TV Stick, Android TV, and Google TV devices.

## Compatibility

This project is compatible with:

- Fire TV Stick 4K (2nd Gen)
- Fire TV Stick 4K Max (2nd Gen)
- Fire TV Sticks that shipped on or before October 2025 with Android
- Android TV devices
- Google TV devices

## Available Clients

### TizenTube

Recommended if you want an experience closer to the original YouTube application.

Repository:\
[https://github.com/reisxd/TizenTube/tree/main](https://github.com/reisxd/TizenTube/tree/main)

### SmartTube

Recommended if you want more configuration options and advanced settings, including:

- Bitrate
- Framerate
- Audio format
- Similar advanced controls

The interface may look different from the traditional YouTube application.

Repository:\
[https://github.com/yuliskov/smarttube](https://github.com/yuliskov/smarttube)

---

# Installation

## Amazon Fire TV Stick

### 1. Enable Developer Options

1. Open **Settings** on your Fire TV Stick.
2. Go to **My Fire TV**.
3. Open **About**.
4. Click the name of your Fire TV Stick repeatedly, approximately seven times, until a message confirms that developer options are enabled.
5. Return to **Settings** and open **Developer Options**.
6. Enable **ADB debugging**.
7. Enable **Apps from Unknown Sources** or **Install from Unknown Sources**.

## Through ADB Command (Most Efficient)

For installing apps directly through ADB without any apk downloading, you can use the commands below. 
**before running the commands please visit this repo to connect the stick via adb to the computer**
https://github.com/srivetriselvan/ADB-guide-for-Amazon-Fire-TV-Stick

### Windows PowerShell

#### SmartTube

```powershell
Invoke-WebRequest -Uri "https://github.com/yuliskov/SmartTube/releases/download/latest/smarttube_stable.apk" -OutFile "$env:TEMP\smarttube.apk"; adb install -r -g "$env:TEMP\smarttube.apk"
```

#### TizenTube

```powershell
Invoke-WebRequest -Uri "https://github.com/reisxd/TizenTubeCobalt/releases/download/v2.0.3/cobalt-arm.apk" -OutFile "$env:TEMP\tizentube.apk"; adb install -r -g "$env:TEMP\tizentube.apk"
```

### Linux (Bash)

#### SmartTube

```bash
curl -L "https://github.com/yuliskov/SmartTube/releases/download/latest/smarttube_stable.apk" -o /tmp/smarttube.apk && adb install -r -g /tmp/smarttube.apk
```

#### TizenTube

```bash
curl -L "https://github.com/reisxd/TizenTubeCobalt/releases/download/v2.0.3/cobalt-arm.apk" -o /tmp/tizentube.apk && adb install -r -g /tmp/tizentube.apk
```

## Through APK

### Download the APK

Download the APK from the **Releases** section of this repository.

### Transfer the APK

Transfer the APK to your Fire TV Stick using one of the following methods:

### Send Files to TV

Use the **Send Files to TV** app from the app store and send the APK from your computer.

### USB Storage

Copy the APK to a USB storage device, connect it to the Fire TV Stick, and use a file manager from the app store to install it.

### 4. Install the Application

Install the APK and launch the application.

---

# Google TV and Android TV

### 1. Enable Developer Options

Enable **Developer Options** on your device.

The process is generally similar to Fire TV Stick.

### 2. Allow Installation from Unknown Sources

Allow installation from unknown sources or enable installation from unknown apps for your file manager.

### 3. Transfer the APK

Transfer the APK to your device using one of the following methods:

- USB storage device
- Send Files to TV
- File manager

### 4. Install the Application

Open the APK using a file manager and install it.

### 5. Launch the Application

Launch the application.

---

# Usage

Enjoy ad-free video streaming and an enhanced viewing experience.

---

# Supporting the Project

If you can afford to support the creators, please consider donating.

We are working hard to provide useful tools and a good experience.

Thank you for your support.

---

# Disclaimer and Legal Information

This project is an independent, open-source alternative client built from the ground up.

## No Copyrighted Code

This repository does not host, distribute, or modify any proprietary binaries, APKs, or copyrighted source code belonging to Google LLC or YouTube.

## Not a Crack

This is not a cracked or patched version of the official YouTube application.

It is a completely separate application that interacts with public APIs.

## Educational and Personal Use

This project is intended for educational purposes, privacy research, and personal customization.

It is not affiliated with, authorized, maintained, or endorsed by YouTube or Google LLC.
