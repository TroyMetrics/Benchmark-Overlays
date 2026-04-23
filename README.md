<h1 align="center">TroyMetrics Benchmark Overlays</h1>
<p align="center">RTSS / RivaTuner Overlays by TroyMetrics 👻</p>

<div align="center">
  <a href="https://youtu.be/O6pbmgcFB5U?si=fzjMaL5J3nlO0qs9">
    <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Video_Thumbnail.png?raw=true" width="850">
  </a>
</div>

# 📖 Overview

A high-precision, **adaptive** performance overlay for RTSS that automatically aligns with your system’s hardware configuration—covering CPU & GPU telemetry, latency, frametime, power delivery, and more. Designed for benchmarkers, gamers, system builders, enthusiasts, and content creators, it unifies dozens of advanced metrics into a single clean, cohesive display. Powered by RTSS and HWiNFO64, the overlay is optimized for accurate, real-time analysis across resolutions from 720p to 4K, whether for gameplay monitoring or formal benchmarking workflows.

<p align="center">
  <a href="#%EF%B8%8F-setup--installation">🚀 SETUP & INSTALLATION</a>
</p>

<div align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/2-Fan_Preview.gif?raw=true" style="max-height: 800px; width: auto;">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/3-Fan_Preview.gif?raw=true" style="max-height: 800px; width: auto;">
</div>

# 💎 Features

<p align="center">
  <a href="#-system-monitoring">🧠 System Monitoring</a>,
  <a href="#%EF%B8%8F-included-presets">🗃️ Included Presets</a>,
  <a href="#-adaptive-cpu-barchart">📊 Adaptive CPU Barchart</a>,
  <a href="#%EF%B8%8F-latency-module-reflex--presentmon-integration">🕹️ Latency Module</a>,
  <a href="#-frame-gen-indicator">🔺 Frame Gen Indicator</a>,
  <a href="#-frametime-graph--stutter-detection">📈 FrameTime Graph</a>,
  <a href="#%EF%B8%8F-thermal-throttle-detection">🌡️ Thermal Throttle Detection</a>,
  <a href="#%EF%B8%8F-power-detector-module-for-supported-gpus">⚡ Power Detector Module</a>,
  <a href="#-organized-layer-structure">🧩 Organized Layers</a>
</p>

## 🧠 System Monitoring
Displays all standard real-time performance metrics including **1% lows**, **average**, and **current FPS**, as well as **CPU and GPU temperatures**, **clock speeds**, **utilization**, **VRAM and system RAM usage**, **latency**, and **power readings** — providing a complete overview of system performance at a glance.

---

## 🗃️ Included Presets

The overlay package includes a curated set of **26 presets**, featuring 11 presets optimized for **1080p** displays, 2 **Color Mod 2-Tone** options, 2 **Animated Rainbow** variants, 2 dedicated **12VHPWR Power Detector-Only** presets, plus multiple **color variants** for instant personalization.

### 🌈 Color Presets

<div align="center">
  <a href="https://youtu.be/v7VLgzUj9RE">
    <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Video_Github.jpg?raw=true" width="850">
  </a>
</div><br><br>

Color presets include: **🟩 Ghostly Green & White (original)**, **🎨 Color Mod 2-Tone**, **🟩 Pure Green**, **🟦 Electric Blue**, **🟨 Bright Yellow**, **🩷 Hot Pink**, **🟧 Pure Orange**, **🟩 Ghostly Green**, and **🌈 Animated Rainbow** (introduced in [v1.10](https://github.com/TroyMetrics/Benchmark-Overlays/releases/tag/v1.10))  

> 🧙‍♂️ **[Learn how to adjust the rainbow animation speed](#-rainbow-animation-speed-sensor-control)**

### 🎨 Color Mod 2-Tone

<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Color_Mod_2-Tone_Preview.png?raw=true">
</p>

The Color **Mod 2-Tone** presets let you transform the overlay’s accent color instantly. Just set a value from **0–100** in the **Color** sensor's Correction formula field and the entire overlay shifts to your chosen hue! — no manual layer editing required. 🪄

Perfect for streamers, benchmarkers, and content creators who want their overlay to match each game’s style, mood, or aesthetic on the fly 🔥

> 🧙‍♂️ **[Learn how to customize the Color Mod 2-Tone preset](#-color-mod-2-tone-color-adjustment)**

---

## 📊 Adaptive CPU Barchart
This fully dynamic layout automatically adjusts for 4 to 24-core CPUs, detecting and displaying only physical cores in properly ordered CPU bar charts. On Intel systems, Performance (P) cores are shown first, followed by Efficiency (E) cores. On AMD, cores are displayed in logical, physical order — providing an accurate and readable view of real CPU utilization during gameplay or stress testing.  
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Dynamic_CPU_Core_Barchart.gif?raw=true" width="75%">
</p>

> 🧙‍♂️ See Also: The [📊 CPU Barchart Automatic Detection](#-cpu-barchart-automatic-detection) section for more details.

---

## 🕹️ Latency Module (Reflex + PresentMon Integration)

The new **Latency Module** has been completely redesigned for [v1.13](https://github.com/TroyMetrics/Benchmark-Overlays/releases/tag/v1.13) to deliver accurate latency telemetry using both **NVIDIA Reflex** and **PresentMon** data sources.  

* Automatically prioritizes **Reflex telemetry** when available (NVIDIA GPUs), with **PresentMon** fallback for all other GPUs — ensuring consistent latency metrics across any system.  
* Displays **GPU Render Latency** and **Frame Pipeline Latency** (Simulation → Render/Display) in real time, providing a detailed look into both CPU and GPU frame processing stages.  
* Uses the latency functions: `reflexlatency(markerFrom, markerTo)` and `presentmonlatency(markerFrom, markerTo)`.  

> 🧙‍♂️ See Also: The [Latency Module Information](#%EF%B8%8F-latency-module-information) section for more details.

<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Latency_Module_New.gif?raw=true">
</p>

---

## 🔺 Frame Gen Indicator
A subtle blinking icon now appears within the **Framerate Module** next to **FPS** when **Frame Gen** is enabled.  
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/FG_Indicator_Icon.gif?raw=true">
</p>  

---

## 📈 FrameTime Graph & Stutter Detection
The **FrameTime Module** provides a real-time visualization of frame pacing, displaying frame times between **0–50 ms** to ensure smooth gameplay analysis. It’s designed to make stutter events easily identifiable during benchmarking or in-game monitoring.

* **Dynamic Stutter Dectection** graph flashes red when a stutter is detected by comparing the current frametime to a **sliding average** (×2 threshold).  
* Includes a **Spike Indicator**, a clean white bar that travels in sync with the frametime graph to visualize frame time spikes (≥ 66.66 ms).
* Adapts dynamically with **Frame Gen**, ensuring accurate frametime reporting while **frame-gen** is enabled.  
  ‣ **FrameGen ON:** switches the graph to display **output-side (display) sensors** eliminating the weird “fat” or “jagged” frametime patterns that older overlays produced when frame generation was active.  
  ‣ **FrameGen OFF:** Operates in classic mode, monitoring the standard game-side frame pacing.
  > 📝 Note: Frametime metrics with **Frame Gen** may lag by ~3 seconds due to PresentMon limitations.  
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/FT_Spike_Indicator.gif?raw=true">
</p>  

---

## 🌡️ Thermal Throttle Detection

Each hardware vendor provides its own **thermal throttle indicators** in **HWiNFO**. These sensors reveal when the CPU or GPU physically reduces clock speed to prevent overheating. The overlay merges those readings into two unified RTSS sensors — `GPUThrottle` and `CPUThrottle` — for consistent detection across all platforms.

**🧠 Detection Sources:**  

<div align="center">

| **Category** | **Vendor** | **HWiNFO Sensor** |
|:-------------:|:-----------:|:------------------|
| GPU 🖥️| NVIDIA | Performance Limit – Thermal |
| GPU 🖥️| AMD | GPU VR GFX Thermal Limit |
| GPU 🖥️| Intel | Hardware Limit ||
| CPU 🔲| Intel | Package / Ring Thermal Throttling |
| CPU 🔲| AMD | Thermal Throttling (PROCHOT EXT) |

</div>

* When **no throttling** is detected → the standard CPU/GPU name is displayed.  
* When **throttling is detected** → the module text changes to a **flashing “GPU/CPU THROTTLE”** alert (as shown below).  

<p align="center">
  <img src="https://raw.githubusercontent.com/TroyMetrics/Benchmark-Overlays/refs/heads/main/assets/images/Thermal_Throttle_Detection_GPU.gif?raw=true" width="50%">
  <br>
  <img src="https://raw.githubusercontent.com/TroyMetrics/Benchmark-Overlays/refs/heads/main/assets/images/Thermal_Throttle_Detection_CPU.gif?raw=true" width="50%">
</p>

---

## ⚡️ Power Detector Module (for supported GPUs)
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Preview.gif?raw=true">
</p>

Designed for **GPUs equipped with 12VHPWR per-pin telemetry**, such as the **ASUS ROG Astral GeForce RTX 5090**, this module provides real-time electrical insight directly within the overlay.  

* Displays **individual 12VHPWR pin amperage** in real time.  
* Calculates and displays **total current draw** and **pin balance percentage**.  
* Uses **status indicator icons** to show **normal, warning, and danger** states.  
* Alerts the user to unsafe conditions such as  
  ‣ **Excessive current** (≥ 9.2 A per pin)  
  ‣ **Dropped pins** (≈ 0 A)  
  ‣ **Power Imbalance** across all 6 pins.  
* Enables **early detection** of potential cable or connector faults before failure occurs.

> ➡️ Details and full safety information are outlined within the ⚡[Power Detector Features & Warnings](#%EF%B8%8F-power-detector-features--warnings) section.

---

## 🧩 Organized Layer Structure

With the layer restructure and naming improvements introduced in [v1.8](https://github.com/TroyMetrics/Benchmark-Overlays/releases/tag/v1.8), user customization is now simpler and more organized than ever.  

<p align="center">
  <img src="https://raw.githubusercontent.com/TroyMetrics/Benchmark-Overlays/refs/heads/main/assets/images/Organized_Layers.gif?raw=true">
</p>

🎨 Got your own design or remix? Share it in the [Guru3D Forum](https://forums.guru3d.com/threads/benchmark-overlays-by-troymetrics-power-detector-module.456668/) — the best ones may even get featured in the official download! 🔥

---

# 🛠️ Setup & Installation

## ✅ Prerequisites

Before setting up the TroyMetrics Benchmark Overlay, make sure the following software is installed and properly configured:

**✅ MSI Afterburner + RivaTuner Statistics Server (RTSS)**

🔽 Download the latest BETA versions of **MSI Afterburner & RTSS** from [www.guru3d.com](https://www.guru3d.com/files-details/msi-afterburner-beta-download.html)
> 📝 Note: The latest beta builds are often shared exclusively on the official Guru3D forums by the developer, Unwinder.
- The MSI Afterburner installer includes **RivaTuner Statistics Server (RTSS)** as a bundle — this is required for the overlay to function.
- During installation, ensure that **✅ RivaTuner Statistics Server** is left **check-marked.**

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

> ⚠️ **Important:** RTSS must be installed on the **C:\\ drive**. Installing it elsewhere (e.g. D:\\) can cause missing or broken overlay icons due to location-dependent resources. See [Issue #7](https://github.com/TroyMetrics/Benchmark-Overlays/issues/7) for details and a potential work around.

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

The overlay was originally designed for 4K displays at a 300% Zoom level for maximum sharpness and pixel clarity.

To adjust scaling, simply use the Zoom slider in RTSS to fit your display.
<div align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/RTSS_Zoom_Example.gif?raw=true">
</div>  
🖥️ For 1080p users, select the 1080p presets — these were fully redesigned to deliver crisp visuals and proper scaling at 1080p resolution. <br><br>

✅ Your overlay is now fully active and ready to use!

> 📌 Jump to [Additional Settings & Information](#-additional-settings--information) or [Setting User-defined Thresholds](#-setting-user-defined-thresholds)

---

# ⚡️ Power Detector Features & Warnings

The Power Detector module is designed for GPUs with 12VHPWR per-pin sensors (such as the ASUS ROG Astral RTX 5090). The Power Detector monitors individual pin amperage, calculating total current, pin balance percentage, and visualizing per-pin status. It dynamically alerts users to unsafe conditions like excessive current (≥9.2 A), dropped pins (≈0 A), and imbalance across power rails—enabling early detection of potential cable or connector issues.

<!-- Power Detector Warnings -->

## **🟢 Normal State**

This status icon indicates that all 12VHPWR pins are operating within expected parameters — with amperage levels safely below the maximum rated specification and well-balanced across all pins. No action is required. ✅

<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Preview.gif?raw=true">
</p>

---

## **🟡 Warning State (Power Imbalance)**

This status icon and alert activates when a significant current disparity is detected between pins (**≤85% power balance**) which may result in hazardous operating conditions under sustained or peak GPU load. The included chart provides a clear visual breakdown of each pin's current deviation from the target or **ideal** per-pin load, calculated dynamically based on total power draw. ⚠️

<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Imbalance_Chart.gif?raw=true">

---

## **🔴 Danger State (Power Alert)**

This status icon and alert is triggered when one or more 12VHPWR pins exceed the maximum rated specification of **9.2 amps**, or drops to **0 amps**, indicating a critical deviation from safe operating conditions that may result in power delivery failure or hardware damage. 💀

<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Power_Alert_Preview.png?raw=true">
</p>

---

## **➖ Sensors Not Available**

This status icon and notice is shown when **per-pin amperage telemetry is unavailable**, either because the **user’s GPU does not support individual 12VHPWR pin sensors**, or because **HWiNFO64 is not running or not reporting sensor data**. In this state, the Power Detector is unable to monitor power integrity or detect pin-specific anomalies.

<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Power_Detector_Sensors_NA.gif?raw=true">
</p>

---

<br><br>

# 🔧 **Additional Settings & Information**

## 🌈 Rainbow Animation Speed Sensor Control

Since **[v1.10](https://github.com/TroyMetrics/Benchmark-Overlays/releases/tag/v1.10)**, the overlay package introduced the **TM Benchmark Overlay – Rainbow** preset — featuring a smooth full-spectrum color-shifting animation across all elements.  

This section explains how to adjust the **rainbow animation speed** using a simple formula in RTSS.

<div align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Rainbow_GPU_Preview.gif?raw=true">
</div>

**✨ Overview**
* The animation speed is driven by the **data source sensor `R1`**.  
* By default, `R1` is configured as a **30-second color loop**, using this formula:

  ```
  (x%30000)/300
  ```

**⚙️ Adjusting the Speed**

If you’d like to make the rainbow cycle faster or slower, simply modify the loop duration in the formula.  

To maintain the full color range without breaking the spectrum cycle, follow this pattern:

<div align="center">

| Desired Loop Duration | Formula |
|------------------------|----------|
| 60 seconds | `(x%60000)/600` |
| 30 seconds *(default)* | `(x%30000)/300` |
| 20 seconds | `(x%20000)/200` |
| 10 seconds | `(x%10000)/100` |
| 5 seconds | `(x%5000)/50` |

</div>

You can experiment with other values as long as the **division remains consistent** with the total loop time.

>⚠️ Note: To the best of my knowledge, a true animated rainbow gradient effect is not currently possible in RTSS unless used as a static image. This preset is a **color-shifting animation**, not a gradient hack.

>👆 UPDATE: Actually [it is possible!](https://github.com/TroyMetrics/TM-GamerStats-1080p), sort of.. lol

**🧭 Example Setup**

Below is an example of the **Rainbow Speed Sensor** configured in RTSS OverlayEditor for a 30 second loop:

![Rainbow Speed Sensor](https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Rainbow_Speed_Sensor.jpg?raw=true)

---

## 🎨 Color Mod 2-Tone Color Adjustment  

The following settings apply specifically to these presets:  

* **TM Benchmark Overlay – Color Mod 2-Tone**  
* **TM Benchmark 1080p – Color Mod 2-Tone**  

The **Color Mod 2-Tone** presets maintain the original TroyMetrics two-tone aesthetic while introducing full dynamic color control. This allows you to instantly customize the overlay’s accent hue without modifying every layer individually.  

To adjust the color:  
1. Open the **Color** sensor in your data source list.  
2. Set a value between **0–100** to define your desired hue across the full RGB spectrum.  

A handy Color Reference Chart is included to guide your inner artist:

<div align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/Color_Reference_Chart.png?raw=true">
</div>  

> 🧙‍♂️ Setting the **Color** sensor to 50 produces a **Cyan** accent color.  

---

## 👤 Setting User-defined Thresholds

The Overlay includes several **animated gauge and indicator elements** that respond dynamically to system performance metrics such as **CPU/GPU clock speeds**, **temperatures**, and **utilization**.  

While the default configuration is tuned for modern high-performance hardware, every threshold can be customized to match your system’s specifications and preferred visuals.

## ⚙️ Setting CPU / GPU **Speed Gauge** Icon Thresholds

Each **speed gauge icon** consists of three layers:  
**Needle**, **Body**, and **Fill** — all visible in the **Layers Edit list** <kbd>Ctrl + Shift + L</kbd> or by navigating to **Layers → Edit list** via the menus as seen here,

<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/User_Defined_Thresholds_Layer_Properties.jpg?raw=true">
</p>

By default, the **GPU Speed Gauge** is configured for a range of **0 – 3000 MHz**, suitable for GPUs such as the RTX 5090.  

If you’re using hardware with lower maximum clock speeds (for example, an RTX 3060 Ti with a 1665 MHz boost clock), you can adjust the range as follows:

1. Select the **Needle** or **Fill** layer.  
2. Open **Embedded animated image settings**.  
3. Locate **Sprite animation maximum, in data source units**.  
4. Change this value from **3000** to your GPU’s max frequency (e.g., **1665 MHz**).

This example shows how to set a GPU speed gauge threshold of 0 to 3000 MHz (this is the default value):
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/User_Defined_Thresholds_GPU_Speed_Gauge.jpg?raw=true">
</p>

This example shows how to set a CPU speed gauge threshold of 0 to 6 GHz (this is the default value):
<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/User_Defined_Thresholds_CPU_Speed_Gauge.jpg?raw=true">
</p>

> 🧙‍♂️ This step must be done for both the needle, and the fill layers so that they match.

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
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/User_Defined_Thresholds_High_Temp_Fire_Icon.jpg?raw=true">
</p>

---

## 🕹️ Latency Module Information

The **Latency Module** includes 4 latency sensors to allow for **PresentMon latency fallback** for non-NVIDIA GPUs: **GpuRenderLatency** and **FramePipelineLatency** (each one has a Reflex and PresentMon variant making it 4 sensors in total).  

  - If the Reflex **GpuRenderLatency** sensor appears *below* its PresentMon counterpart in the data source list, Reflex latency telemetry will take priority and display automatically (requires Nvidia GPU).  
  - To disable Reflex for consistent cross-platform comparisons, simply move its entry **above** the PresentMon sensor in the Data source list — may be preferable if comparing benchmark results between NVIDIA vs AMD systems, or monitoring Sim-to-Display latency performance.

**🧙‍♂️ How It Works**

The Data source functions `presentmonlatency(markerFrom, markerTo)` and `reflexlatency(markerFrom, markerTo)` calculate the latency between two defined markers within the current frame, as [explained here](https://forums.guru3d.com/threads/msi-ab-rtss-development-news-thread.412822/page-224#post-6223060). Refer to the charts below for a clearer understanding of how each marker pair is used. In this overlay, the formula "**min(**`presentmonlatency(1,8)`**, 999.9)**" clamps latency values to a maximum of **999.9 ms** purely for aesthetic consistency and to prevent overflow during abnormal spikes.

**🟦 PresentMon Latency Markers**

| **Index** | **Marker Name** | **Meaning** |
|:--:|:--|:--|
| 0 | `input_sample` | Input event (used only when Reflex Analyzer hardware is available) |
| 1 | `cpu_busy_start` | Game simulation and logic start — the CPU begins processing the next frame |
| 2 | `cpu_busy_end` | Simulation and draw-call submission complete — CPU work for the frame ends |
| 3 | `present_start` | CPU issues the `Present()` call to the graphics API |
| 4 | `present_end` | `Present()` call completes — frame submitted to the OS / driver queue |
| 5 | `gpurender_start` | GPU begins executing the rendering commands for the frame |
| 6 | `gpurender_end` | GPU finishes rendering — frame ready for presentation |
| 8 | `display` | Display scan-out / frame becomes visible on screen |

**🧙‍♂️ Notes:**
- PresentMon collects **software-level API timestamps** (DXGI/D3D12/Vulkan) directly from the graphics stack.  
- Default latency formulas used in this overlay:
  - **GpuRenderLatency (GPU Render Latency):** `presentmonlatency(5,6)`  
  - **FramePipelineLatency (Simulation → Display):** `presentmonlatency(1,8)`  
- PresentMon measures **Simulation-to-Display**, but does **not** include driver-internal queueing or scheduling latency.  
- Marker `0` (`input_sample`) exists for compatibility with Reflex Analyzer hardware but does not output data in standard PresentMon telemetry.

**🟩 NVIDIA Reflex Latency Markers**

| **Index** | **Marker Name** | **Meaning** |
|:--:|:--|:--|
| 0 | `input_sample` | Input event (Reflex Analyzer hardware only) |
| 1 | `simulation_start` | CPU simulation start — begins processing game logic and input |
| 2 | `simulation_end` | Simulation complete — CPU is ready to hand off work to render submission |
| 3 | `rendersubmit_start` | CPU begins submitting rendering commands to the GPU via the driver |
| 4 | `rendersubmit_end` | CPU finishes submitting all rendering commands to the driver |
| 5 | `present_start` | CPU issues the `Present()` call |
| 6 | `present_end` | The `Present()` call completes and returns control to the CPU |
| 7 | `driver_start` | Frame enters the driver queue — waiting for GPU scheduling or availability |
| 8 | `driver_end` | Frame leaves the driver queue — driver submission is complete and GPU is ready to start |
| 9 | `osrenderqueue_start` | OS-level render queue start (e.g., compositor or presentation manager) |
| 10 | `osrenderqueue_end` | OS-level render queue end |
| 11 | `gpurender_start` | GPU begins executing rendering commands (hardware render start) |
| 12 | `gpurender_end` | GPU finishes rendering the frame (hardware render complete) |

**🧙‍♂️ Notes:**
- Reflex provides **driver-level and GPU-level telemetry** inserted below the graphics API, allowing precise capture of CPU, driver, and GPU timing stages.  
- Default latency formulas used in this overlay:
  - **GpuRenderLatency (GPU Render Latency):** `reflexlatency(11,12)`  
  - **FramePipelineLatency (Simulation → GPU Render End):** `reflexlatency(1,12)`  
- With Reflex Analyzer hardware, marker `0` expands measurement to include **input latency** and **display response**, enabling complete *click-to-photon* analysis.  
  - If you have compatible Analyzer hardware, you can modify your formula to begin at marker `0` to capture **true end-to-end latency**.

---

## 🧠 CPU Barchart Automatic Detection

The overlay now detects physical CPU cores using HWiNFO’s **“Core # T0 Effective Clock”** sensors for AMD and **“P-core # T0 Effective Clock”** + **“E-core # T0 Effective Clock”** sensors for Intel (found under **Core Effective Clocks**).  
These sensors map **1:1 to real physical cores**, ensuring accurate detection across AMD and Intel hybrid CPUs and preventing incorrect barchart selection.

The sensor **`PhysicalCoreCount`** uses the formula below to determine how many physical cores are valid and automatically select the correct CPU Usage Barchart:

```txt
if(validate("CPU Core Count Override"),"CPU Core Count Override",(C0+C1+C2+C3+C4+C5+C6+C7+C8+C9+C10+C11+C12+C13+C14+C15+C16+C17+C18+C19+C20+C21+C22+C23+C24+C25+C26+C27+C28+C29+C30+C31+P0+P1+P2+P3+P4+P5+P6+P7+P8+P9+P10+P11+P12+P13+P14+P15+P16+P17+P18+P19+P20+P21+P22+P23+E0+E1+E2+E3+E4+E5+E6+E7+E8+E9+E10+E11+E12+E13+E14+E15+E16+E17+E18+E19+E20+E21+E22+E23))
```

> 🧙‍♂️ For automatic detection to function, all corresponding **“P/E/Core # T0 Effective Clock”** sensors must remain **visible (not hidden)** in HWiNFO64.

If you prefer manual control—or if you don’t use HWiNFO—you can override automatic detection using the  
**`CPU Core Count Override`** sensor to directly choose which barchart the overlay displays.

> 🧙‍♂️ See Also: The **[📊 CPU Core Count Override Sensor](#-cpu-core-count-override-sensor)** section for more details.

---

## 📊 CPU Core Count Override Sensor

A new override sensor now allows users to **manually select which CPU barchart is displayed**.  
To use it, open **Data sources (`Ctrl + D`)** and enter your physical CPU core count into the **Correction formula**.

📊 Supported charts: **4, 6, 8, 10, 12, 14, 16, 20, 24**.  

> 📝 Note: This feature is intended for users who don’t run HWiNFO or who prefer full manual control.  
> After entering your core count, be sure to **Save your preset**, so the override persists and you won’t need to re-enter it later.

<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/CPU_Core_Count_Override_Sensor.png?raw=true">
</p>

> 🧙‍♂️ For **Automatic CPU Core Detection** (HWiNFO), the Correction formula must remain **empty**.

---

## ℹ️ CPU Barchart Status Message

The status message **“HWiNFO not running: Start HWiNFO or set CPU Core Count Override.”** appears when the overlay cannot determine your system’s physical core count. It is shown only when the following is true:

- **HWiNFO64 is not running** / **Shared Memory Support** is disabled  
- **No value has been assigned** in the **[CPU Core Count Override](#-cpu-core-count-override-sensor)** sensor  

It displays this status message to prompt the user to either launch HWiNFO64 (or enable Shared Memory Support) or manually assign their CPU core count using the **[CPU Core Count Override Sensor](#-cpu-core-count-override-sensor)**

<p align="center">
  <img src="https://github.com/TroyMetrics/Benchmark-Overlays/blob/main/assets/images/CPU_Barchart_Info_Message.png?raw=true">
</p>

Once HWiNFO is running—or an override value is provided—the barchart will display normally.

---

# ❤️ A Note to the Community

This overlay was built with the goal of creating a fully adaptable performance overlay that works seamlessly across a wide range of hardware — from 720p laptops to high-end 4K benchmark rigs.

It is designed to automatically adjust to your system with minimal manual tweaking, especially when paired with HWiNFO for real-time hardware detection. As a full-time (HVAC/Plumbing) service tech with limited PC hardware on hand, I rely heavily on community feedback to keep improving the project.

If you encounter any issues — CPU core ordering, overlapping layers, incorrect detection logic, missing support for a specific CPU, or anything that feels off — please open an Issue on GitHub. Screenshots are incredibly helpful and greatly speed up fixes.

Your reports and suggestions directly help this project grow.
Thank you for testing, supporting, and helping make the TroyMetrics Benchmark Overlay better for everyone. 🙏

# 🧙‍♂️ More from TroyMetrics

If you enjoy this overlay, check out some other designs:

- [📌 (New) **TroyMetrics Benchmark Overlays 2**](https://github.com/TroyMetrics/Benchmark-Overlays-2)
- [📌 **TM GamerStats 1080p**](https://github.com/TroyMetrics/TM-GamerStats-1080p)

*(This list will continue to expand as more designs are released.)*

🚀 Enjoy benchmarking with **TroyMetrics Benchmark Overlays**!  

## ☕ **Enjoying the overlay?**  
**Fuel my coffee addiction — [support me with a virtual latte!](https://buymeacoffee.com/justinraabe)**
