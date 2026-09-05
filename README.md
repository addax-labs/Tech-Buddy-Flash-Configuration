# 🌐 ADDAX Labs - Tech Buddy V1 Setup Portal

Welcome to the official setup portal codebase for the **Tech Buddy V1**—an open-source, agnostic AI desktop companion engineered by **ADDAX Labs**. 

This interface allows users to safely configure their hardware devices via a standard Google Chrome or Microsoft Edge browser window using the native **Web Serial API**. No heavy software installations or command-line coding required.

---

## ✨ Features

- **Bring-Your-Own-Key (BYOK) Architecture:** Eliminates data privacy liabilities and rate limits by flashing user-owned API credentials straight to the hardware.
- **Universal Multi-Model Support:** Fully compatible with endpoints for **Google Gemini, OpenAI, Groq, and Anthropic**.
- **100% Zero-Cloud Frontend:** Runs entirely client-side in the browser. Credentials bypass external servers and go straight over the Type-C wire into the ESP32.
- **Premium Cyberpunk/Pastel UI:** Clean, responsive dark-theme design matching the ADDAX Labs design philosophy.

---

## 🛠️ How It Works

1. **Connect:** Connect the Tech Buddy V1 to your machine via a USB Type-C cable.
2. **Authorize:** Click **"Connect Tech Buddy"** to launch the browser's native serial device handshaking port at `115200` baud rate.
3. **Provision:** Enter local Wi-Fi parameters, your target AI provider's API URL, your private API key, and the model string.
4. **Flash:** Hit **"Flash Configuration"** to stream a clean JSON payload directly into the ESP32's non-volatile storage (`Preferences.h`).

---

## 🚀 Deployment

Because this portal relies strictly on native browser scripts without external node packages or framework dependencies, you can deploy it instantly:
- Run it locally by double-clicking the `setup.html` file.
- Deploy it globally for free using **GitHub Pages**.

---

## ⚖️ License & Open Source
Developed by **ADDAX Labs**. Built for the global maker and open-hardware community. 
