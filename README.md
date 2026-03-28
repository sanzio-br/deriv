# 🔱 Apex Trading Suite
**High-Frequency Algorithmic Trading Bots for Deriv/Binary.com**

This repository contains a collection of specialized, client-side trading bots built with HTML5, TailwindCSS, and Native WebSockets.

## 📂 Project Structure
* `html/`: Contains the standalone executable bot files.
* `assets/`: UI components and design language specifications.

## 🤖 Available Bots

| Bot Name | Strategy | Signal Logic | Status |
| :--- | :--- | :--- | :--- |
| **[V100 Turbo Dual-Mode](#-v100-turbo-dual-mode)** | Serial Triple-Entry | Digit Over/Under | ✅ Stable |
| **V200 Pulse** | Reversion | Mean Reversion | 🛠️ In Dev |

---

## 🚀 V100 Turbo Dual-Mode
**The flagship high-speed serial executor.**

V100 Turbo utilizes a dual-zone trigger system to maximize win probability across the full digit spectrum (0-9).

### ⚙️ Core Logic
* **Zone A (Bullish):** Triggers **Digit Over** on digits `0, 1, 2`.
* **Zone B (Bearish):** Triggers **Digit Under** on digits `7, 8, 9`.
* **The Gap:** Digits `3, 4, 5, 6` act as a safety buffer (no trades).

### 🛠️ Installation & Usage
1. Navigate to the `html/` directory.
2. Open `v100-turbo.html` in any modern web browser.
3. Enter your **Deriv API Token**.
4. Set your Stake and Martingale (Recommended: `11.0` for full recovery).
5. Click **Connect** and then **Start Turbo**.

### 📊 Advanced Analytics
The V100 Turbo includes a real-time **Serial Analytics Engine**:
* **Contract ID Tracking:** Prevents double-counting and race conditions.
* **Entry/Exit Logging:** Precise verification of every tick result.
* **Digit Frequency Map:** Visualizes live market bias.

---

## ⚠️ Disclaimer
Trading involves significant risk. These bots are experimental tools. Always test on a **Demo Account** before using real capital. The Martingale strategy can lead to rapid balance depletion.