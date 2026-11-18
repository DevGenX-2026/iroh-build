<!-- ВСТАВЬТЕ СЮДА СКОПИРОВАННЫЙ КОД БЕЙДЖА С PRODUCT HUNT -->

# 🏠 AIHome — Local Smart Home, Security & Voice Assistant Hub

**AIHome** is a 100% local, privacy-first smart home and personal assistant hub built in **Rust** for Windows, paired with an encrypted P2P Android companion app.

No monthly subscriptions. No cloud dependency for cameras, voice, or family chats. Everything runs directly on your own PC.

---

## ✨ Key Features

* 🎙 **100% Offline Bilingual Voice Assistant (EN / RU):**
  * Powered by **VOSK** with customizable wake words, custom word-correction dictionary, and hands-free text dictation.
  * Launch games/apps, control media, manage browser/YouTube tabs, and trigger smart home scenes by voice.
  * Optional **Voice ID** speaker filtering (20-band Goertzel frequency analysis) so the assistant only responds to your voice.

* 👁 **Local Computer Vision & Security Guard:**
  * **Real-Time Face Recognition:** Greets family members automatically, tracks home presence, and captures snapshots of unknown visitors (can be named by voice or from your phone).
  * **Interactive Camera Zones:** Draw custom zones on camera feeds to automatically turn linked lights on/off when someone enters or leaves.
  * **Air Mouse (Touchless Hand Control):** Control your Windows cursor and clicks (LMB, RMB, Dwell) with hand gestures using **ONNX Runtime + MoveNet** and OneEuro smoothing.

* 💡 **Unified Smart Home & Automation:**
  * Direct local TCP/UDP control and Wi-Fi provisioning for smart bulbs (with smooth brightness fading).
  * **Tuya Cloud** integration for smart relays and switches.
  * Custom scenes (e.g., *Cinema*, *Sleep*) and weekly day/time schedules.

* 📱 **Encrypted P2P Android Companion (via Iroh / QUIC):**
  * Connect phones directly to your PC by scanning a one-time QR code (with admin approval & granular per-device permissions).
  * Live **H.264** camera streaming, remote touchpad/keyboard, and Push-to-Talk voice commands.
  * Self-hosted **Family Chat** with photo/video/audio sharing and automatic storage quota management.
  * Direct 1-on-1 & group **audio/video calls** relayed through your home PC.
  * Privacy-first **Family Geofencing** with 24-hour route map generation (OpenStreetMap / MapTiler / Stadia Maps).

---

## 🛠 Tech Stack

* **Core & UI:** Rust, `eframe` / `egui`
* **P2P Networking:** Iroh (QUIC)
* **Speech & Audio:** VOSK, `cpal`, Goertzel DSP filter
* **Computer Vision:** ONNX Runtime (MoveNet), OpenH264
* **IoT:** Local UDP/TCP protocols + Tuya OpenAPI (HMAC-SHA256)

---

## 📥 Download

Grab the latest Windows build and Android APK from the **[Releases](https://github.com)** page.
