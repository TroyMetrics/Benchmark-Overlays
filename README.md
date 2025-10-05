<h1 align="center">Benchmark Overlay</h1>
<p align="center">RTSS / RivaTuner Overlay by TroyMetrics 👻</p>

<div align="center">
  <a href="https://youtu.be/O6pbmgcFB5U?si=fzjMaL5J3nlO0qs9">
    <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Video_Thumbnail.png" width="850">
  </a>
</div>

# Overview

A clean and professional RTSS overlay built for high-visibility performance benchmarking. This fully dynamic overlay balances vital metrics with visual clarity and adapts to any Intel or AMD CPU (up to 24 cores), ensuring correct core ordering for accurate real-time hardware insight during gameplay or stress tests.

<div align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/2-Fan_Preview.gif" style="max-height: 800px; width: auto;">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/3-Fan_Preview.gif" style="max-height: 800px; width: auto;">
</div>
<br><br>

**Now includes 14 Presets:** Benchmark 3-Fan Power Detector, Benchmark 2-Fan, Benchmark 3-Fan, 12VHPWR Power Detector (Power Detector Only), 3 Presets with Latency Modules, and [7 Color Options](https://github.com/TroyMetrics/Benchmark-Overlays#-new-color-options-available)

# Features

## 📊 Adaptive CPU Barchart
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Dynamic_CPU_Core_Barchart.gif" width="75%">
</p>

This fully dynamic layout automatically adjusts for 4 to 24-core CPUs, detecting and displaying only physical cores in properly ordered CPU bar charts. On Intel systems, Performance (P) cores are shown first, followed by Efficiency (E) cores. On AMD, cores are displayed in logical, physical order — providing an accurate and readable view of real CPU utilization during gameplay or stress testing.

## 🧠 System Monitoring
Includes 1% lows, average, and current FPS metrics, GPU and CPU temperatures, clock speeds, average effective clock speeds, utilization, VRAM usage, system RAM usage, latency metrics and more.

## 🕹️ Latency Module (Render | Sim-to-Render Latency)
Added below the Frame Time Graph, now showing **Render Latency** and **Sim-to-Render Latency** in milliseconds.
- Dynamic values are centered for cleaner aesthetics given the layout while the titles (LAT and MS) remain static for less distraction. 
- Metrics are capped at **999 ms** to prevent huge number strings from shooting across the screen during certain scenarios (e.g. when Alt-Tabbing in and out of a game).
<p align="center">
  <img src="https://raw.githubusercontent.com/TroyMetrics/Benchmark-Overlays/refs/heads/main/assets/images/Latency_Module.gif">
</p>

## 🔺Frame Gen Indicator
  • A subtle blinking icon now appears next to **FPS** when Frame Gen is active.  
  • While active, the Frame Time Graph switches to the updated mode for accurate pacing display.  
> Note: Frametime metrics with Frame Gen may lag by ~3 seconds due to PresentMon limitations.

## ⚡️ Power Detector Module (for supported GPUs)
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Preview.gif" width="100%">
</p>

Designed for **GPUs equipped with 12VHPWR per-pin telemetry**, such as the **ASUS ROG Astral GeForce RTX 5090**, this module provides real-time electrical insight directly within the overlay.  

- Displays **individual 12VHPWR pin amperage** in real time.  
- Calculates and displays **total current draw** and **pin balance percentage**.  
- Uses adaptive color indicators to show **normal, warning, and danger** states.  
- Alerts the user to unsafe conditions such as  
  ‣ **Excessive current** (≥ 9.2 A per pin)  
  ‣ **Dropped pins** (≈ 0 A)  
  ‣ **Imbalance** across 12 V rails.  
- Enables **early detection** of potential cable or connector faults before failure occurs.

> ➡️ Details and full safety information are outlined within the [⚡Power Detector Features & Warnings](#%EF%B8%8F-power-detector-features--warnings) section.

## 🌈 Color Options

<div align="center">
  <a href="https://youtu.be/v7VLgzUj9RE">
    <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Video_Github.jpg" width="850">
  </a>
</div>

New color customization options have expanded significantly since [v1.9](https://github.com/TroyMetrics/Benchmark-Overlays/releases/tag/v1.9), making it easier than ever to personalize your overlay.  

Available color presets now include: **Ghostly Green & White (original)**, **Pure Green**, **Electric Blue**, **Bright Yellow**, **Hot Pink**, **Pure Orange**, **Ghostly Green**, and the new **Rainbow preset** introduced in [v1.10](https://github.com/TroyMetrics/Benchmark-Overlays/releases/tag/v1.10).  

> ➡️ See also: **[How to adjust the rainbow animation speed](#-rainbow-animation-speed-sensor-control)**

## 🧩 Organized Layer Structure

With the layer restructure and naming improvements introduced in [v1.8](https://github.com/TroyMetrics/Benchmark-Overlays/releases/tag/v1.8), user customization is now simpler and more organized than ever.  

<p align="center">
  <img src="https://raw.githubusercontent.com/TroyMetrics/Benchmark-Overlays/refs/heads/main/assets/images/Organized_Layers.gif"><br><br>
</p>

Got your own design or remix? Share it in the [Guru3D Forum](https://forums.guru3d.com/threads/benchmark-overlays-by-troymetrics-power-detector-module.456668/) — the best ones may even get featured in the official download! 🔥

# ⚡️ Power Detector Features & Warnings

The Power Detector module is designed for GPUs with 12VHPWR per-pin sensors (such as the ASUS ROG Astral RTX 5090). The Power Detector monitors individual pin amperage, calculating total current, pin balance percentage, and visualizing per-pin status. It dynamically alerts users to unsafe conditions like excessive current (≥9.2 A), dropped pins (≈0 A), and imbalance across power rails—enabling early detection of potential cable or connector issues.

<!-- Power Detector Warnings -->

## **✅ Normal State**

<p align="left">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Status_Normal.png">
</p>

This status icon indicates that all 12VHPWR pins are operating within expected parameters — with amperage levels safely below the maximum rated specification and well-balanced across all pins. No action is required. ✅<br><br>

---

## **⚠️ Warning State (Power Imbalance)**

<p align="left">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Status_Warning.png">
</p>

This status icon and alert activates when a significant current disparity is detected between pins (**≤85% power balance**) which may result in hazardous operating conditions under sustained or peak GPU load. The included chart provides a clear visual breakdown of each pin's current deviation from the target or **ideal** per-pin load, calculated dynamically based on total power draw. ⚠️<br>
<p align="left">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Imbalance_Chart.gif">

---

## **💀 Danger State (Power Alert)**

<p align="left">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Status_Danger.png">
</p>

This status icon and alert is triggered when one or more 12VHPWR pins exceed the maximum rated specification of **9.2 amps**, or drops to **0 amps**, indicating a critical deviation from safe operating conditions that may result in power delivery failure or hardware damage. 🔴<br>
<p align="left">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Power_Alert_Preview.png">
</p>

---
  
## **➖ Sensors Not Available**

<p align="left">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Status_NA.png">
</p>

This status icon and notice is shown when **per-pin amperage telemetry is unavailable**, either because the **user’s GPU does not support individual 12VHPWR pin sensors**, or because **HWiNFO64 is not running or not reporting sensor data**. In this state, the Power Detector is unable to monitor power integrity or detect pin-specific anomalies.
<p align="left">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Sensors_NA.gif">
</p>

# 🛠️ Setup & Installation

## ✅ Prerequisites

Before setting up the TroyMetrics Benchmark Overlay, make sure the following software is installed and properly configured:

**✅ MSI Afterburner + RivaTuner Statistics Server (RTSS)**

🔽 Download the latest BETA versions of **MSI Afterburner & RTSS** from [www.guru3d.com](https://www.guru3d.com/files-details/msi-afterburner-beta-download.html)
> 📝 Note: The latest beta builds are often shared exclusively on the official Guru3D forums by the developer, Unwinder.
- The MSI Afterburner installer comes bundled with **RivaTuner Statistics Server (RTSS)** — this is required for the overlay to function.
- During installation, ensure that **✅ RTSS** is **check-marked.**

---

**✅ HWiNFO64**

🔽 Download the latest version of **HWiNFO64** from [www.hwinfo.com](https://www.hwinfo.com/download/)
> **🛡️ Recommended for Power Users:** Consider purchasing the paid version to remove the **12-hour Shared Memory Support time limit** and **enable automatic updates.**

**⚙️ Important Configuration Steps:**
1. Launch HWiNFO64 (Sensors Only) and click the **`[Sensors]`** button
2. Click the Cogwheel button in the bottom-right ⚙️ **`"Configure Sensors"`**
3. In the new window, click **`[Main Settings]`** (bottom-right)
4. Make sure **`✔ Shared Memory Support`** is enabled

> ✅ Shared Memory Support is required for RTSS to read sensor data from HWiNFO — especially critical for modules like the **12VHPWR Power Detector** (per-pin amperage monitoring).

---

## 🛠️ Setup Instructions

> ⚠️ **Important:** RTSS must remain installed on the **C:\\ drive**. Installing it elsewhere (e.g. D:\\) can cause missing or broken overlay icons due to location-dependent resources. See [Issue #7](https://github.com/TroyMetrics/Benchmark-Overlays/issues/7) for details and a potential work around.

**1. 📦 Extract and Prepare Files**
- Open the downloaded package: **`TroyMetrics Benchmark Overlays`**
- In a **new File Explorer window**, navigate to your **`C:\` drive**

**2. 📁 Copy Overlay Files to RTSS**
- **Drag and drop** (or **copy/paste**) the folder named **`Program Files (x86)`** from the downloaded package directly into your **`C:\` drive**
- If prompted for admin permission:
  - ✅ Check **"Do this for all current items"**
  - ✅ Click **"Continue"**

> This step places the overlay files in the correct RTSS directory.

---

**3. 🔤 Install the Required Font**
- Navigate to:  
  `C:\Program Files (x86)\RivaTuner Statistics Server\Fonts`
- Double-click to install: **Adderley Bold.ttf**

> **Font credit:** *Adderley* by gorohovskiy  
> Licensed under the SIL Open Font License. All rights reserved by the original creator.

---

**4. ⚙️ Enable OverlayEditor in RTSS**
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

**5. 🎛 Load the Overlay in OverlayEditor**
1. With **OverlayEditor.dll** enabled, double-click it or click **`[Setup]`** after high-lighting it 
2. In the Overlay Editor window:
   - Go to the **`Layouts`** tab → Click **`Load`**
   - Select one of the **`TroyMetrics Benchmark Overlays`** → Click **`Open`**

---

**6. 🧠 Apply Master Settings (Important)**
- Since **RTSS Beta 7.3.2**, you can now use **`Ctrl + Shift + M`** to apply the overlay’s master layout settings. Otherwise, follow the steps below for manual application.
- Back in the **Layouts** tab → Click **`Edit`**
- In the **Overlay Properties** window:
  - Click **`[Master Settings]`**
  - Click **`Yes`** when prompted
  - Click **`OK`** to finalize

---

**7. 🔍 Adjust Zoom Slider (if necessary)**
🔍 This overlay was designed for 4K displays at a 300% Zoom level to ensure sharp visuals. You can resize the entire overlay by adjusting the Zoom slider within RTSS to best fit your screen.
<div align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/RTSS_Zoom_Example.gif" style="max-height: 800px; width: auto;">
</div>

✅ Your overlay is now fully active and ready to use!

---

# 🔧 **Optional Settings**

## 🌈 Rainbow Animation Speed Sensor Control

Since **[v1.10](https://github.com/TroyMetrics/Benchmark-Overlays/releases/tag/v1.10)**, the overlay package introduces a new preset — **TM Benchmark Overlay – Rainbow** — featuring a smooth full-spectrum color-shifting animation across all elements.  

This section explains how to adjust the **rainbow animation speed** using a simple formula in RTSS.

![Rainbow GPU Preview](https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Rainbow_GPU_Preview.gif)

**✨ Overview**
* The animation speed is driven by the **data source sensor `R1`**.  
* By default, `R1` is configured as a **30-second color loop**, using this formula:

  ```
  (x%30000)/300
  ```

**⚙️ Adjusting the Speed**

If you’d like to make the rainbow cycle faster or slower, simply modify the loop duration in the formula.  
To maintain the full color range without breaking the spectrum cycle, follow this pattern:

| Desired Loop Duration | Formula |
|------------------------|----------|
| 60 seconds | `(x%60000)/600` |
| 30 seconds *(default)* | `(x%30000)/300` |
| 20 seconds | `(x%20000)/200` |
| 10 seconds | `(x%10000)/100` |
| 5 seconds | `(x%5000)/50` |

You can experiment with other values as long as the **division remains consistent** with the total loop time.

>⚠️ Note: To the best of my knowledge, a true animated rainbow gradient effect is not currently possible in RTSS unless used as a static image. This preset is a **color-shifting animation**, not a gradient hack.

**🧭 Example Setup**

Below is an example of the **Rainbow Speed Sensor** configured in RTSS OverlayEditor for a 30 second loop:

![Rainbow Speed Sensor](https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Rainbow_Speed_Sensor.jpg)

## 👤 Setting User-defined Thresholds

The Overlay includes several **animated gauge and indicator elements** that respond dynamically to system performance metrics such as **CPU/GPU clock speeds**, **temperatures**, and **utilization**.  

While the default configuration is tuned for modern high-performance hardware, every threshold can be customized to match your system’s specifications and preferred visuals.

## ⚙️ GPU & CPU Clock **Speed Gauge** Threshold

Each **speed gauge icon** consists of three layers:  
**Needle**, **Body**, and **Fill** — all visible in the **Layers Edit list** <kbd>Ctrl + Shift + L</kbd> or by navigating to **Layers → Edit list** via the menus as seen here,

<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/User_Defined_Thresholds_Layer_Properties.jpg" width="75%">
</p>

By default, the **GPU Speed Gauge** is configured for a range of **0 – 3000 MHz**, suitable for GPUs such as the RTX 5090.  
If you’re using hardware with lower maximum clock speeds (for example, an RTX 3060 Ti with a 1665 MHz boost clock), you can adjust the range as follows:

1. Select the **Needle** or **Fill** layer.  
2. Open **Embedded animated image settings**.  
3. Locate **Sprite animation maximum, in data source units**.  
4. Change this value from **3000** to your GPU’s max frequency (e.g., **1665 MHz**).

This example shows how to set a GPU speed gauge threshold of 0 to 3000 MHz (this is the default value):
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/User_Defined_Thresholds_GPU_Speed_Gauge.jpg" width="75%">
</p>

This example shows how to set a CPU speed gauge threshold of 0 to 6 GHz (this is the default value):
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/User_Defined_Thresholds_CPU_Speed_Gauge.jpg" width="75%">
</p>

> 📝 Note: This step must be done for both the needle, and the fill layers so that they match.

---

## 🔥 **High Temperature Indicator (Fire Icon)** Threshhold

The **animated fire icon** visually warns when component temperatures exceed a defined limit.

By default, this threshold is set to **≥ 83 °C** for both CPU and GPU, controlled via the **Dynamic Color** options.

Inside the **Dynamic color** configuration:
- **0 – 100 °C:** Layer color is set to **0% opacity black** (invisible).  
- **≥ 100 °C:** Layer color transitions to **100% opacity white**, activating the animated fire icon.

To customize:
1. Select the **Fire Icon** layer.  
2. Open **Dynamic color** settings.  
3. Adjust the threshold value to your preferred activation point (e.g., 90 °C, 95 °C, or 100 °C).

This example demonstrates how the Dynamic Color threshold is set to make the fire icon visible when GPU temperature ≥ 100 °C.
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/User_Defined_Thresholds_High_Temp_Fire_Icon.jpg" width="75%">
</p>

# 🎉 You're All Set!
Enjoy benchmarking with **TroyMetrics Benchmark Overlays**!  
If you have any questions or feedback, feel free to open an issue or contact me via GitHub. I’m happy to help.

☕ **Enjoying the overlay?**  
**Fuel my coffee addiction — [support me with a virtual latte!](https://buymeacoffee.com/justinraabe)**
