╔═══════════════════════════════════════════════════════════╗
║           HYPER AX MANAGER — v1.0.0                      ║
║     Premium AI Gaming Performance Plugin                  ║
║     Developer: Gailo Willy                                ║
║     Platform : AxeronManager (Non-Root Plugin)            ║
╚═══════════════════════════════════════════════════════════╝

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 WHAT THIS PLUGIN DOES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 • Forces display to run at maximum supported Hz (120/144/165)
 • Removes 60 FPS and 90 FPS caps from games at system level
 • Sets all CPU cores to performance governor at max frequency
 • Forces GPU (Adreno/Mali) to maximum clock speed
 • Disables thermal throttle daemon safely
 • Enables Thermal Guard watchdog (auto safe-mode at 58°C)
 • Reduces input/touch latency to near-zero
 • Optimizes TCP/IP stack for online gaming (ping reduction)
 • Clears background apps when game is active
 • Reduces audio buffer to 192 samples (low-latency audio)
 • All tweaks survive reboot via BOOT_COMPLETED service

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 SUPPORTED DEVICES
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 • Snapdragon 7xx / 8xx series (Adreno GPU)
 • MediaTek Dimensity 8xxx / 9xxx (Mali GPU)
 • Exynos 2xxx / S5E series (Mali GPU)
 • Android 10 (API 29) and above
 • No root required (AxManager non-root mode)
 • Optional: root enhances thermal daemon control

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 HOW TO INSTALL
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 1. Open AxeronManager app
 2. Tap "Plugins" tab
 3. Tap the "+" / Install button
 4. Select HyperAxManager.zip
 5. Tap FLASH / INSTALL
 6. Wait for install log — look for success message
 7. Reboot device (OR tap Action button for immediate apply)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 AFTER INSTALL
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 • Tweaks auto-apply 10 seconds after boot
 • Tap ACTION button in AxManager to manually re-apply
 • WebUI Dashboard available inside AxManager plugin view
 • Logs saved to: /data/local/tmp/hyperax_apply.log

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 FPS UNLOCK RESULTS (Expected)
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 Game                        Before     After
 ─────────────────────────────────────────────
 Mobile Legends              60 FPS  →  120 FPS
 PUBG Mobile                 60 FPS  →  90 FPS
 Call of Duty Mobile         60 FPS  →  120 FPS
 Free Fire                   60 FPS  →  120 FPS
 Genshin Impact              60 FPS  →  60 FPS (app limit)
 Roblox                      60 FPS  →  120 FPS
 Fortnite Mobile             60 FPS  →  120 FPS

 Note: Some games enforce their own FPS cap in-app.
 Enable "High Frame Rate" in each game's graphics settings
 for best results. This plugin unlocks the SYSTEM limit.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 THERMAL SAFETY
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 42°C  → Warning logged (no action)
 47°C  → Slight freq reduction (5%)
 52°C  → Moderate reduction (15%)
 58°C  → SAFE MODE: schedutil governor, GPU relaxed
 63°C  → EMERGENCY: powersave mode, thermal re-enabled
 45°C  → Resume performance mode

 The Thermal Guard daemon runs in background at all times.
 It auto-recovers performance once device cools down.
 NO bootloop risk — system thermal is never fully disabled.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 CONFIG CUSTOMIZATION
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 Edit files in the config/ folder to customize behavior:
 • config/fps_unlock.conf   — per-game FPS limits
 • config/thermal_control.conf — temp thresholds
 • config/cpu_tweak.conf   — governor & scheduler
 • config/gpu_tweak.conf   — GPU frequency policy
 • config/refresh_rate.conf — Hz unlock options

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 WARNINGS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 ⚠ Battery drain will INCREASE at max performance mode.
   Use a power bank or charger during long sessions.

 ⚠ Device will run WARMER than normal.
   Ensure good airflow. Remove phone case if overheating.

 ⚠ Some OEM apps (MIUI, Samsung GameBooster) may conflict.
   Disable built-in game optimization apps for best results.

 ⚠ This plugin does NOT modify system partitions.
   It is fully safe and reversible. Uninstall restores defaults.

 ⚠ Not responsible for abnormal battery wear from sustained
   max-performance usage.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 CREDITS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 Developer  : Gailo Willy
 Engine     : Hyper Ax Manager v1.0.0
 Platform   : AxeronManager Plugin System
 BusyBox    : Compiled from Magisk project
 Special Thanks: AxManager developer (fahrez182)

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 LOG FILE LOCATIONS
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
 Main log   : /data/local/tmp/hyperax_apply.log
 Game boost : /data/local/tmp/hyperax_gameboost.log
 Thermal    : /data/local/tmp/hyperax_thermal.log
 Action     : /data/local/tmp/hyperax_action.log
