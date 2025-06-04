# Benchmark Overlay
RTSS / RivaTuner Overlay by TroyMetrics

<p align="center">
  <img src="https://github.com/user-attachments/assets/63aac7bf-cca7-4dff-83d9-80d76f170ab3" style="height: 800px; width: auto;">
  <img src="https://via.placeholder.com/50x1/00000000/00000000?text=+" width="50" height="1">
  <img src="https://github.com/user-attachments/assets/27129669-e580-4d93-909e-fcc7153045ed" style="height: 800px; width: auto;">
</p>

## Overview

A clean and professional RTSS overlay built for high-visibility performance benchmarking. This fully dynamic overlay balances vital metrics with visual clarity and adapts to any Intel or AMD CPU (up to 24 cores), ensuring correct core ordering for accurate real-time hardware insight during gameplay or stress tests.

Includes 3 versions:

### 🌀 2 & 3-Fan GPU Designs 
<p align="center">
  <img src="https://github.com/user-attachments/assets/5c7e5766-204d-49f4-b3c3-2b4b5c3c4489" width="50%"><img src="https://github.com/user-attachments/assets/bc181ff0-c0d8-47ec-aee4-763d81b0ef16" width="50%">
</p>

### ⚡️ Power Detector Module  
<p align="center">
  <img src="https://github.com/user-attachments/assets/c561f0b4-f033-4f23-9040-41aeb8e561e8" width="100%">
</p>

The Power Detector module is designed for GPUs with 12VHPWR per-pin sensors (such as the ASUS ROG Astral RTX 5090). The Power Detector monitors individual pin amperage, calculating total current, pin balance percentage, and visualizing per-pin status. It dynamically alerts users to unsafe conditions like excessive current (≥9.2 A), dropped pins (≈0 A), and imbalance across power rails—enabling early detection of potential cable or connector issues.

<!-- Power Detector Warnings -->

## <img src="https://github.com/user-attachments/assets/07ff59f3-0c26-4207-b185-7590b36065b2" width="20"> Normal

Indicates that all 12VHPWR pins are operating within expected parameters — with amperage levels safely below the maximum rated specification and well-balanced across all pins. No action is required.<br>

## <img src="https://github.com/user-attachments/assets/179036d2-6af9-4d4e-a040-22ef446c96f4" width="20"> Power Alert

This alert is triggered when one or more 12VHPWR pins exceed the maximum rated specification of **9.2 amps per pin**, or drop to **0 amps**, indicating a critical deviation from safe operating conditions that may result in power delivery failure or hardware damage.<br>
<p align="center">
  <img src="https://github.com/user-attachments/assets/daa67fbb-4e5a-465c-b924-4bf38ce30b2c" width="100%"><br><br>
</p>

## <img src="https://github.com/user-attachments/assets/b7ef7484-18ce-41db-b825-20abe24c1963" width="20"> Major Power Imbalance

This alert activates when a significant current disparity is detected between pins (**≤75% power balance**) which may result in hazardous operating conditions under sustained or peak GPU load.<br>
<p align="center">
  <img src="https://github.com/user-attachments/assets/576eaef5-6b23-4abb-a564-92408089ab1b" width="100%"><br><br>

## <img src="https://github.com/user-attachments/assets/6475dda5-6371-435d-9249-acd530e47ce5" width="20"> Power Imbalance

This warning indicates a moderate deviation in current between pins, signaling potential strain or emerging imbalance in power delivery that should be monitored to maintain safe 12VHPWR compliance.<br>
<p align="center">
  <img src="https://github.com/user-attachments/assets/bec57c2e-f822-469b-9cdf-721af80f07d1" width="100%"><br><br>
  </p>
  
## <img src="https://github.com/user-attachments/assets/2df78461-22ad-4623-ae51-f9eb5ec6d1d3" width="20"> Sensors Not Available<br>

This notice is shown when **per-pin amperage telemetry is unavailable**, either because the **user’s GPU does not support individual 12VHPWR pin sensors**, or because **HWiNFO64 is not running or not reporting sensor data**. In this state, the Power Detector is unable to monitor power integrity or detect pin-specific anomalies.
<p align="center">
  <img src="https://github.com/user-attachments/assets/c7246cbb-188f-415d-980b-d56929bdb248" width="100%">
</p>



<!-- CPU Core Barcharts Gif -->
![Image](https://github.com/user-attachments/assets/8b294ad3-d9fd-4407-aea5-0a7353c15dbf)
