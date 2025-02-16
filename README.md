# Lenovo Ideapad 530s Hackintosh (macOS Sonoma)

This repository contains the EFI folder for creating a Hackintosh on a **Lenovo Ideapad 530s**. It is set up with **OpenCore** and is fully configured to run macOS **Sonoma 14.7.2 (23H311)**. The setup supports the essential hardware components, including Intel Wi-Fi and Bluetooth.

### Hardware Specifications:
- **Laptop Model**: Lenovo Ideapad 530s
- **Storage**: **Samsung MZVLW256HEHP-000L2** 256GB SSD
  - **Capacity**: 256,06 GB (256.060.514.304 bytes)
  - **TRIM Support**: Yes
  - **Model**: SAMSUNG MZVLW256HEHP-000L2
- **RAM**: 16GB (upgraded from 8GB)
- **Processor**: Intel Core i7-8550U (Quad-Core, 2.0 GHz)
- **Graphics**: Intel UHD Graphics 620 (1536 MB, working)

### Hardware Overview:
- **Model Name**: MacBook Pro
- **Model Identifier**: MacBookPro16,3
- **Processor Name**: Quad-Core Intel Core i7-8550U
- **Processor Speed**: 2 GHz
- **Number of Processors**: 1
- **Total Number of Cores**: 4
- **L2 Cache (per Core)**: 256 KB
- **L3 Cache**: 8 MB
- **Hyper-Threading Technology**: Disabled
- **Memory**: 16 GB
- **System Firmware Version**: 2069.0.0.0.0
- **OS Loader Version**: 580.140.1~51

### macOS Version:
- **macOS Version**: **Sonoma 14.7.2 (23H311)**

### Bootloader:
- **Bootloader**: OpenCore

### BIOS Settings:
Before installing macOS, make sure to configure your BIOS settings as follows:

- **Disable discrete GPU (dGPU)**: Ensure the system uses the integrated graphics.
- **Disable Intel SGX** (Software Guard Extensions).
- **Disable Intel Secure Boot**: This is necessary for compatibility with macOS.

### Wi-Fi & Bluetooth Setup:
- **Wi-Fi**: The Intel Wi-Fi is supported using [itlwm](https://github.com/OpenIntelWireless/itlwm) and managed via [HeliPort](https://github.com/OpenIntelWireless/HeliPort).
- **Bluetooth**: Intel Bluetooth is working out-of-the-box with macOS support.

### NOT WORKING:
- **Fingerprint Scanner**: Not working.
- **Nvidia MX150**: Not supported.

### Installation Notes:
1. Make sure to prepare your USB installer with OpenCore for macOS Sonoma 14.7.2.
2. Apply the EFI folder from this repository to the EFI partition of your USB drive.
3. Boot using OpenCore, and select the macOS installer to begin the installation.

For detailed guidance on installing and configuring OpenCore for Hackintosh setups, refer to the [OpenCore Installation Guide](https://dortania.github.io/OpenCore-Install-Guide/).

### Credits:
- [OpenCore](https://github.com/acidanthera/OpenCorePkg) for bootloader support.
- [itlwm](https://github.com/OpenIntelWireless/itlwm) and [HeliPort](https://github.com/OpenIntelWireless/HeliPort) for Intel Wi-Fi support.
- [Intel Bluetooth](https://github.com/OpenIntelWireless/IntelBluetoothFirmware) support.
