# 🌿 MySensor Hub — ESP32-S3 N16R8 Firmware Installer

Web-based installer for the MySensor ESP32-S3 hub (**N16R8** boards: 16MB flash / 8MB PSRAM), built for use with [Cannabis Planner](https://play.google.com/store/apps/details?id=com.ivangospocic.cannabisplanner) — a 100% offline, privacy-focused grow tracker.

This installer flashes the MySensor firmware directly to your ESP32-S3 board using [ESP Web Tools](https://esphome.github.io/esp-web-tools/) — no software installation required.

---

## ⚠️ Which version do I need?

| Your board | Installer |
|---|---|
| **ESP32-S3 N16R8** (16MB flash / 8MB PSRAM) | **This page** |
| Standard 4MB ESP32 | [mysensor-instal](https://cannabisplanner.github.io/mysensor-instal/) |

Flashing the wrong firmware on a board will leave it unable to boot. If you are not sure which board you have, check the label on the module (e.g. `ESP32-S3-WROOM-1-N16R8`).

---

## 📺 Video Tutorial

Watch the full step-by-step setup, from flashing the firmware to connecting the sensor to the app:

▶️ [Watch on YouTube](https://www.youtube.com/watch?v=27Nmx-xaarU)

*(The video shows the standard ESP32 installer; the steps are the same for N16R8.)*

---

## 🚀 How to Install

1. **Connect your ESP32-S3** to your computer via USB cable.
2. Open this page in **Google Chrome** or **Microsoft Edge** on a **desktop computer**:
   👉 [https://cannabisplanner.github.io/mysensor-instal-n16r8/](https://cannabisplanner.github.io/mysensor-instal-n16r8/)
3. Click **Install Firmware** and select your device's serial/COM port.
4. Wait for flashing to complete (this can take a few minutes).
5. Once done, open the **Cannabis Planner** app on your phone and connect to your sensor from the **Environment** tab.

> ⚠️ **This only works in Chrome or Edge on desktop (Windows/Mac/Linux/ChromeOS).**
> It does **not** work on mobile browsers, or in Firefox/Safari, due to Web Serial API limitations.

### Troubleshooting

- **No port appears in the list:** try a different USB cable (some are charge-only) or another USB port. On Windows you may need a CP210x or CH340 driver.
- **Linux:** add your user to the `dialout` group (`sudo usermod -aG dialout $USER`), then log out and back in.
- **Flashing does not start:** put the board into download mode — hold the **BOOT** button, press **RESET** briefly, release BOOT, then click Install again.
- **Erase device:** the installer offers to erase the device first. This is recommended for a first install, but it also removes saved WiFi settings and stored history.

---

## 📱 Get the App

Cannabis Planner is available for free on Google Play:

<a href="https://play.google.com/store/apps/details?id=com.ivangospocic.cannabisplanner">
  <img src="https://play.google.com/intl/en_us/badges/static/images/badges/en_badge_web_generic.png" alt="Get it on Google Play" height="60"/>
</a>

---

## 🔧 Supported Hardware

This firmware is built for **ESP32-S3 N16R8** modules (16MB flash / 8MB PSRAM). For standard 4MB ESP32 boards, use the [4MB installer](https://cannabisplanner.github.io/mysensor-instal/).

---

## 🔒 Privacy First

Cannabis Planner works 100% offline — no cloud sync, no accounts, no tracking. All sensor data stays on your device.

---

## ⚠️ Disclaimer

This project is intended for educational and planning purposes only. Users are responsible for complying with local laws and regulations.
