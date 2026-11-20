# PrintOps Station

A portable, high-speed Windows desktop print station and operator console built with Python, PyQt6, and Flask. Designed for walk-in print shops to automate customer file intake over local Wi-Fi/hotspot and Windows Bluetooth, route print jobs directly to physical USB printers, and track daily print logs.

## Key Features

- **Dual Wireless File Intake:** Accepts customer uploads via a local Wi-Fi/hotspot web portal (QR code access) alongside automated background Windows Bluetooth file reception (`fsquirt.exe`).
- **Fast Operator Shortcuts:** Single-key keyboard controls (`1`–`9` for copies, `c` for Color, `b` for Black & White) with safe queue management for duplicate filenames.
- **Direct Windows Spooler Routing:** Binds directly to physical USB printer ports (`USB001`–`USB006`, `DOT4_001`) using `win32print` for automatic Color vs. Black & White routing.
- **Local Audit & Revenue Logging:** Stores daily copy counts, timestamps, and transaction summaries in an embedded local SQLite database (`data/print_station.db`).
- **Zero-Install Portable Build:** Runs directly from an extracted folder on Windows 10/11 (64-bit) with no Python installation or setup wizard required.

## Quick Start (Windows x64)

1. Go to the **[Releases](https://github.com/Iviande/PrintOps-Station/releases)** page and download the latest `PrintOps_Station-v1.0.0-win64.zip`.
2. Right-click the downloaded `.zip` file and select **Extract All...** to a folder on your PC (e.g., `C:\PrintOps_Station`).
3. Open the extracted `PrintOps_Station` folder and double-click **`PrintOps_Station.exe`**.
4. On first launch, the application automatically creates its local `data/` directory and SQLite database.

## System Requirements

- **OS:** Windows 10 or Windows 11 (64-bit / x64)
- **Hardware:** Physical USB-connected printer(s) and Wi-Fi/hotspot or Bluetooth adapter# PrintOps-Station
