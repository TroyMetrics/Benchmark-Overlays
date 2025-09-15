<h1 align="center">Benchmark Overlay</h1>
<p align="center">RTSS / RivaTuner Overlay by TroyMetrics 👻</p>

<div align="center">
  <a href="https://youtu.be/O6pbmgcFB5U?si=fzjMaL5J3nlO0qs9">
    <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Video_Thumbnail.png" width="850">
  </a>
</div>
<h1 align="center"><a href="https://github.com/TroyMetrics/Benchmark-Overlay/releases/latest">⬇️ Download</a></h2>

# Overview

A clean and professional RTSS overlay built for high-visibility performance benchmarking. This fully dynamic overlay balances vital metrics with visual clarity and adapts to any Intel or AMD CPU (up to 24 cores), ensuring correct core ordering for accurate real-time hardware insight during gameplay or stress tests.

<div align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/2-Fan_Preview.gif" style="max-height: 800px; width: auto;">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/3-Fan_Preview.gif" style="max-height: 800px; width: auto;">
</div>
<br><br>

**Now includes 7 Presets:** Benchmark 3-Fan Power Detector, Benchmark 2-Fan, Benchmark 3-Fan, 12VHPWR Power Detector (Power Detector Only), and 3 Presets with Latency Modules!

# Features

## 📊 Adaptive CPU Barchart
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Dynamic_CPU_Core_Barchart.gif" width="75%">
</p>

This fully dynamic layout automatically adjusts for 8 to 24-core CPUs, detecting and displaying only physical cores in properly ordered CPU bar charts. On Intel systems, Performance (P) cores are shown first, followed by Efficiency (E) cores. On AMD, cores are displayed in logical, physical order — providing an accurate and readable view of real CPU utilization during gameplay or stress testing.

## 🧠 System Monitoring
Includes 1% lows, average, and current FPS metrics, GPU and CPU temperatures, clock speeds, average effective clock speeds, utilization, VRAM usage, system RAM usage and more.

## 🕹️ Latency Module (Render | Sim-to-Render Latency)
Added below the Frame Time Graph, now showing **Render Latency** and **Sim-to-Render Latency** in milliseconds.
  • Dynamic values are centered for cleaner aesthetics given the layout while the titles (LAT and MS) remain static for less distraction. 
  • Metrics are capped at **999 ms** to prevent huge number strings from shooting across the screen during certain scenarios (e.g. when Alt-Tabbing in and out of a game).
<p align="center">
  <img src="https://raw.githubusercontent.com/TroyMetrics/Benchmark-Overlays/refs/heads/main/assets/images/Latency_Module.gif">
</p>

## 🔺Frame Gen Indicator
  • A subtle blinking icon now appears next to **FPS** when Frame Gen is active.  
  • While active, the Frame Time Graph switches to the updated mode for accurate pacing display.  
> Note: Frametime metrics with Frame Gen may lag by ~3 seconds due to PresentMon limitations.

# ⚡️ Power Detector Module  
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Preview.gif" width="100%">
</p>

The Power Detector module is designed for GPUs with 12VHPWR per-pin sensors (such as the ASUS ROG Astral RTX 5090). The Power Detector monitors individual pin amperage, calculating total current, pin balance percentage, and visualizing per-pin status. It dynamically alerts users to unsafe conditions like excessive current (≥9.2 A), dropped pins (≈0 A), and imbalance across power rails—enabling early detection of potential cable or connector issues.

<!-- Power Detector Warnings -->

## <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Status_Normal.png" width="20"> **Normal** <br>
Indicates that all 12VHPWR pins are operating within expected parameters — with amperage levels safely below the maximum rated specification and well-balanced across all pins. No action is required.<br><br>

## <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Status_Danger.png" width="20"> **Power Alert** <br>
This alert is triggered when one or more 12VHPWR pins exceed the maximum rated specification of **9.2 amps**, or drops to **0 amps**, indicating a critical deviation from safe operating conditions that may result in power delivery failure or hardware damage.<br>
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Power_Alert_Preview.png" width="100%"><br><br>
</p>

## <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Status_Warning.png" width="20"> **Major Power Imbalance** <br>
This alert activates when a significant current disparity is detected between pins (**≤85% power balance**) which may result in hazardous operating conditions under sustained or peak GPU load. The included chart provides a clear visual breakdown of each pin's current deviation from the target or **ideal** per-pin load, calculated dynamically based on total power draw.<br>
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Imbalance_Chart.gif?raw=true" width="100%"><br><br>
  
## <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Status_NA.png" width="20"> **Sensors Not Available** <br>

This notice is shown when **per-pin amperage telemetry is unavailable**, either because the **user’s GPU does not support individual 12VHPWR pin sensors**, or because **HWiNFO64 is not running or not reporting sensor data**. In this state, the Power Detector is unable to monitor power integrity or detect pin-specific anomalies.
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Sensors_NA.gif" width="100%"><br><br>
</p>

# 🛠️ Setup & Installation

## ✅ Prerequisites

Before setting up the TroyMetrics Benchmark Overlay, make sure the following software is installed and properly configured:

---

### 🧰 MSI Afterburner + RivaTuner Statistics Server (RTSS)

- Download the latest BETA versions of **MSI Afterburner & RTSS** from [www.guru3d.com](https://www.guru3d.com/files-details/msi-afterburner-beta-download.html)
- The installer includes **RivaTuner Statistics Server (RTSS)** — this is required for the overlay to function.
- During installation, ensure that **✅ RTSS is check-marked**.

---

### 📊 HWiNFO64

- Download the latest version of **HWiNFO64** from [www.hwinfo.com](https://www.hwinfo.com/download/)
- 🛡️ **Recommended for Power Users:** Consider purchasing the paid version to:
  - Remove the **12-hour Shared Memory Support time limit**
  - Enable automatic updates
- **Important Configuration Step:**
  1. Launch HWiNFO64 and click the **`[Sensors]`** button
  2. Click the Cogwheel button in the bottom-right ⚙️ **`"Configure Sensors"`**
  3. In the new window, click **`[Main Settings]`** (bottom-right)
  4. Make sure **`✔ Shared Memory Support`** is enabled

> ✅ Shared Memory Support is required for RTSS to read sensor data — especially critical for modules like the **12VHPWR Power Detector** (per-pin amperage monitoring).

---

## Setup Instructions

### 1. 📦 Extract and Prepare Files
- Open the downloaded package: **`TroyMetrics Benchmark Overlays`**
- In a **new File Explorer window**, navigate to your **`C:\` drive**

### 2. 📁 Copy Overlay Files to RTSS
- **Drag and drop** (or **copy/paste**) the folder named **`Program Files (x86)`** from the downloaded package directly into your **`C:\` drive**
- If prompted for admin permission:
  - ✅ Check **"Do this for all current items"**
  - ✅ Click **"Continue"**

This step places the overlay files in the correct RTSS directory.

---

### 3. 🔤 Install the Required Font
- Navigate to:  
  `C:\Program Files (x86)\RivaTuner Statistics Server\Fonts`
- Double-click to install: **Adderley Bold.ttf**

> **Font credit:** *Adderley* by gorohovskiy  
> Licensed under the SIL Open Font License. All rights reserved by the original creator.

---

### 4. ⚙️ Enable OverlayEditor in RTSS
1. Launch **RivaTuner Statistics Server (RTSS)**  
2. Click the **`[Setup]`** button  
3. In the new window, go to the **Plugins** tab:
   - ✅ Enable **`OverlayEditor.dll`**
   - ✅ (Optional but recommended) Enable **`HotkeyHandler.dll`**
     - Highlight **`HotkeyHandler.dll`** & Click **`[Setup]`** at the bottom to assign hotkeys:
       - **Toggle On-Screen Display**: e.g., `Home`
       - **Begin/End Recording**: e.g., `Page Up / Page Down`

> ⚠️ If you’ve already assigned hotkeys in **MSI Afterburner**, you can skip this step or unassign them there. Only **one program** should manage OSD hotkeys to avoid conflicts.

---

### 5. 🎛 Load the Overlay in OverlayEditor
1. With **OverlayEditor.dll** enabled, double-click it or click **`[Setup]`** after high-lighting it 
2. In the Overlay Editor window:
   - Go to the **`Layouts`** tab → Click **`Load`**
   - Select one of the **`TroyMetrics Benchmark Overlays`** → Click **`Open`**

---

### 6. 🧠 Apply Master Settings (Important)
- Since **RTSS Beta 7.3.2**, you can now use **`Ctrl + Shift + M`** to apply the overlay’s master layout settings. Otherwise, follow the steps below for manual application.
- Back in the **Layouts** tab → Click **`Edit`**
- In the **Overlay Properties** window:
  - Click **`[Master Settings]`**
  - Click **`Yes`** when prompted
  - Click **`OK`** to finalize

---

### 7. 🔍 Adjust Zoom Slider (if necessary)
🔍 This overlay was designed for 4K displays at a 300% Zoom level to ensure sharp visuals. You can resize the entire overlay by adjusting the Zoom slider within RTSS to best fit your screen.
<div align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/RTSS_Zoom_Example.gif" style="max-height: 800px; width: auto;">
</div>

✅ Your overlay is now fully active and ready to use!

---

### 🎉 You're All Set!
Enjoy benchmarking with **TroyMetrics Benchmark Overlays**!  
If you have any questions or feedback, feel free to open an issue or contact me via GitHub. I’m happy to help.
### ☕ **Enjoying the overlay?**  
**Fuel my coffee addiction — [support me with a virtual latte!](https://buymeacoffee.com/justinraabe)**
