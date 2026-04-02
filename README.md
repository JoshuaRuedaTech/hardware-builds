# hardware-builds

## Kali-Tail Wi-Fi Pn testing build
# 🐍 Kali Linux on Raspberry Pi Zero W (Kali Tail) Setup & Troubleshooting

## ✅ Goal
Boot a portable Kali Linux image on the Raspberry Pi Zero W with working Wi-Fi for penetration testing or stealth use.

---

## 🔧 Flashing & Setup

### 🖥️ 1. **Flash Kali Image**
- Use [Raspberry Pi Imager](https://www.raspberrypi.com/software/) or **BalenaEtcher**.
- Choose the appropriate **Kali ARM image** for Raspberry Pi.
- When flashing:
  - ✅ Set **SSID** and **Wi-Fi Password**.
  - ✅ Set **country code** (e.g., `US`).
  - ✅ Enable **SSH** (optional but useful for headless setups).

This step creates a working `/etc/wpa_supplicant/wpa_supplicant.conf` automatically.

---

## ⚠️ Wi-Fi Troubleshooting

### 🧠 Symptom
- Wi-Fi **interface exists** and **can scan** networks.
- But **won't connect** to any SSID manually.

### 🧪 Checklist

- [x] **Confirmed interface exists**
  ```bash
  iw dev
## END

**Building and Setting up my Custom Gaming PC 250420**
## Parts List

- **Motherboard**: ASUS TUF B650-PLUS WIFI
    
- **GPU**: ASUS RTX 5070 Ti OC Gaming
    
- **CPU**: AMD Ryzen 5 7600X
    
- **CPU Cooler**: AMD Wraith RGB
    
- **RAM**: Corsair Vengeance DDR5 32GB
    
- **SSD**: Samsung 990 PRO w/Heatsink 2TB M.2 NVMe
    
- **Mouse**: Redragon M612 Predator RGB Gaming Mouse
    
- **Keyboard**: Redragon K552 65% Mechanical Gaming Keyboard
    
- **Monitor**: TUF Gaming VG3A Series 27" WQHD
    
- **Power Supply**: Corsair RM850X FM 80+ Gold ATX3
    
- **Case**: MUSEWTEX PC Case ATX w/ 6 PWM ARGB Fans
    

## ⚙️ Setup Journey: From Windows Woes to Linux Triumph

The initial plan was to run **Windows 11** on this new gaming rig. After flashing the Windows ISO on a USB and entering the installer, everything looked fine — until it didn't.

Despite multiple reinstalls, BIOS adjustments, and partition wipes, Windows would either:

- Fail to detect the Samsung 990 NVMe SSD
    
- Loop endlessly into BIOS
    
- Or throw bootloader errors even after seemingly successful installs
    

We spent over **12 hours** trying to make Windows work, using diskpart, adjusting UEFI/CSM/Secure Boot settings, and even recreating the USB using different tools.

### The Turning Point: Pop!_OS

Frustrated with Microsoft's roadblocks, we decided to flash **Pop!_OS (NVIDIA version)** instead.

- Within minutes, the live environment **recognized the NVMe SSD instantly**
    
- The installer completed successfully **on the first try**
    
- Wi-Fi, GPU, and peripherals **all worked out of the box**
    

It was such a contrast that it honestly felt emotional — Pop!_OS turned a 12-hour Windows nightmare into a **15-minute Linux dream.**

## 🎮 Post-Install Gaming Setup

With the system running beautifully on Pop!_OS, we:

- Installed **Steam (Flatpak)** with Proton enabled
    
- Installed **ProtonUp-Qt** and added the latest **GE-Proton** version
    
- Enabled **GameMode** and **MangoHUD** for performance + overlays
    
- Verified hardware performance with **glmark2**, scoring **35487**
    
- Installed **Cyberpunk 2077**, running at **1440p Ultra with DLSS and ray tracing**
    

Pop!_OS proved to be not just an alternative, but a **superior** gaming OS for this build.

## 🔧 Notes for Future Reference

- Disable Secure Boot for Pop!_OS to boot correctly (due to shim signature)
    
- Use UEFI boot only — no legacy mode needed
    
- MangoHUD + gamemoderun make it easy to monitor FPS, temps, and load
    
- GE-Proton via ProtonUp-Qt makes the biggest compatibility difference
    

## ✅ Verdict

If you're building a high-end gaming PC and want **performance, stability, and control**, Pop!_OS is a phenomenal choice. It just works — and it works beautifully.

---

**Next Steps**: Document Steam performance benchmarks, AI tool compatibility, and modding setups.
