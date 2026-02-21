
<div align="center">

```
██╗  ██╗██╗   ██╗██████╗ ███████╗██████╗
██║  ██║╚██╗ ██╔╝██╔══██╗██╔════╝██╔══██╗
███████║ ╚████╔╝ ██████╔╝█████╗  ██████╔╝
██╔══██║  ╚██╔╝  ██╔═══╝ ██╔══╝  ██╔══██╗
██║  ██║   ██║   ██║     ███████╗██║  ██║
╚═╝  ╚═╝   ╚═╝   ╚═╝     ╚══════╝╚═╝  ╚═╝

    ██╗  ██╗██╗  ██╗
    ██║  ██║╚██╗██╔╝
    ███████║ ╚███╔╝
    ██╔══██║ ██╔██╗
    ██║  ██║██╔╝ ██╗
    ╚═╝  ╚═╝╚═╝  ╚═╝  M A N A G E R
```

### 🎮 **Premium AI Gaming Performance Plugin** 🎮

![Version](https://img.shields.io/badge/Version-v1.0.0-00d4ff?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-AxeronManager-7c3aed?style=for-the-badge)
![Android](https://img.shields.io/badge/Android-10%2B-00ff88?style=for-the-badge)
![Root](https://img.shields.io/badge/Root-Not%20Required-ff9500?style=for-the-badge)

> 👨‍💻 **Developer:** Gailo Willy &nbsp;|&nbsp; 📱 **Platform:** AxeronManager (Non-Root Plugin)

</div>

---

## ⚡ What This Plugin Does

> 🚀 **One plugin. Maximum performance. Zero compromise.**

| # | Feature | Description |
|---|---------|-------------|
| 🖥️ | **Max Refresh Rate** | Forces display to run at maximum supported Hz (120 / 144 / 165) |
| 🎯 | **FPS Cap Removal** | Removes 60 FPS and 90 FPS caps from games at system level |
| 🧠 | **CPU Boost** | Sets all CPU cores to performance governor at max frequency |
| 🎨 | **GPU Boost** | Forces GPU (Adreno / Mali) to maximum clock speed |
| 🌡️ | **Thermal Control** | Disables thermal throttle daemon safely |
| 🛡️ | **Thermal Guard** | Smart watchdog — auto safe-mode activates at 58°C |
| 👆 | **Touch Latency** | Reduces input / touch latency to near-zero |
| 🌐 | **Network Boost** | Optimizes TCP/IP stack for online gaming (ping reduction) |
| 🧹 | **RAM Cleaner** | Clears background apps when game is active |
| 🔊 | **Audio Latency** | Reduces audio buffer to 192 samples (low-latency sound) |
| 🔄 | **Persistent** | All tweaks survive reboot via `BOOT_COMPLETED` service |

---

## 📱 Supported Devices

```
┌─────────────────────────────────────────────────────────┐
│  🔵  Snapdragon 7xx / 8xx series    →  Adreno GPU       │
│  🟢  MediaTek Dimensity 8xxx / 9xxx →  Mali GPU         │
│  🟣  Exynos 2xxx / S5E series       →  Mali GPU         │
│  🤖  Android 10 (API 29) and above                      │
│  🔓  No Root Required  (AxManager non-root mode)        │
│  ✨  Optional: Root enhances thermal daemon control      │
└─────────────────────────────────────────────────────────┘
```

---

## 📥 How to Install

```
Step 1  →  📲  Open AxeronManager app
Step 2  →  🔌  Tap the "Plugins" tab
Step 3  →  ➕  Tap the "+" / Install button
Step 4  →  📂  Select  HyperAxManager.zip
Step 5  →  ⚡  Tap  FLASH / INSTALL
Step 6  →  📋  Wait for install log — look for success message
Step 7  →  🔁  Reboot device  OR  tap Action button for immediate apply
```

---

## ✅ After Install

| Action | Result |
|--------|--------|
| 🔁 **After Reboot** | Tweaks auto-apply **10 seconds** after boot |
| 🎮 **Action Button** | Tap **ACTION** in AxManager to manually re-apply tweaks |
| 🌐 **WebUI Dashboard** | Live dashboard available inside AxManager plugin view |
| 📄 **Logs** | Saved to `/data/local/tmp/hyperax_apply.log` |

---

## 🎮 FPS Unlock Results (Expected)

| 🎮 Game | Before | After | Status |
|--------|--------|-------|--------|
| Mobile Legends | 60 FPS | **120 FPS** | ✅ Unlocked |
| PUBG Mobile | 60 FPS | **90 FPS** | ✅ Unlocked |
| Call of Duty Mobile | 60 FPS | **120 FPS** | ✅ Unlocked |
| Free Fire | 60 FPS | **120 FPS** | ✅ Unlocked |
| Genshin Impact | 60 FPS | **60 FPS** | ⚠️ App Limit |
| Roblox | 60 FPS | **120 FPS** | ✅ Unlocked |
| Fortnite Mobile | 60 FPS | **120 FPS** | ✅ Unlocked |

> 💡 **Note:** Some games enforce their own FPS cap in-app.
> Enable **"High Frame Rate"** in each game's graphics settings for best results.
> This plugin unlocks the **SYSTEM limit** — in-app settings still apply.

---

## 🌡️ Thermal Safety System

> 🛡️ **Smart Thermal Guard runs in background 24/7 — your device is always protected.**

```
  42°C  🟡  ──  Warning logged          (no performance change)
  47°C  🟠  ──  Slight freq reduction   (−5% clocks)
  52°C  🔶  ──  Moderate reduction      (−15% clocks)
  58°C  🔴  ──  SAFE MODE               (schedutil governor, GPU relaxed)
  63°C  🆘  ──  EMERGENCY               (powersave mode, thermal re-enabled)
  45°C  🟢  ──  Resume performance mode (auto-recovery)
```

> ✅ **NO bootloop risk** — system thermal is never fully disabled.
> The guard **auto-recovers** performance once the device cools down.

---

## ⚙️ Config Customization

Edit files in the `config/` folder to fine-tune behavior:

| 📄 Config File | ⚙️ Controls |
|---------------|------------|
| `config/fps_unlock.conf` | Per-game FPS limits & engine overrides |
| `config/thermal_control.conf` | Temperature thresholds & daemon settings |
| `config/cpu_tweak.conf` | Governor, scheduler & cluster tuning |
| `config/gpu_tweak.conf` | GPU frequency policy & rendering pipeline |
| `config/refresh_rate.conf` | Hz unlock options & per-app overrides |

---

## ⚠️ Warnings & Disclaimers

> **Please read before using!**

🔋 **Battery Drain**
> Performance mode will **increase battery consumption.**
> Use a power bank or charger during long gaming sessions.

🌡️ **Device Temperature**
> Your device will run **warmer than normal.**
> Ensure good airflow. Remove phone case if overheating occurs.

📱 **OEM App Conflicts**
> Some OEM apps (MIUI Game Turbo, Samsung GameBooster, ColorOS Game Space) **may conflict.**
> Disable built-in game optimization apps for best results.

🔒 **System Safety**
> This plugin does **NOT modify system partitions.**
> It is fully **safe and reversible.** Uninstall restores all defaults.

⚡ **Responsibility**
> Developer is **not responsible** for abnormal battery wear
> from sustained max-performance usage.

---

## 📊 Log File Locations

```bash
📋  Main Apply Log   →  /data/local/tmp/hyperax_apply.log
🎮  Game Boost Log   →  /data/local/tmp/hyperax_gameboost.log
🌡️  Thermal Log      →  /data/local/tmp/hyperax_thermal.log
👆  Action Log       →  /data/local/tmp/hyperax_action.log
```

---

## 👨‍💻 Credits

```
┌──────────────────────────────────────────────────────┐
│                                                      │
│   👨‍💻  Developer     :  Gailo Willy                   │
│   ⚙️  Engine        :  Hyper Ax Manager v1.0.0       │
│   📱  Platform      :  AxeronManager Plugin System   │
│   📦  BusyBox       :  Compiled from Magisk project  │
│   🙏  Special Thanks:  fahrez182 (AxManager dev)     │
│                                                      │
└──────────────────────────────────────────────────────┘
```

---

<div align="center">

**🔥 MAX FPS &nbsp;|&nbsp; MAX Hz &nbsp;|&nbsp; MAX PERFORMANCE 🔥**

*Made with ❤️ by Gailo Willy*

</div>
