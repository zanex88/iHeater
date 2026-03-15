# iHeater Integration via Klipper and Home Assistant

This guide describes how to set up the iHeater as a standalone Klipper MCU (without a printer mainboard) and integrate its chamber control macro into Home Assistant based on the active print material.

## 1. Raspberry Pi Setup with KIAUH

1. Flash **Raspberry Pi OS Lite (64-bit)** to an SD card (configure Wi-Fi and SSH credentials via Raspberry Pi Imager).
2. Boot the Pi, connect via SSH, and install KIAUH:
   ```bash
   sudo apt-get update && sudo apt-get install git -y
   git clone [https://github.com/dw-0/kiauh.git](https://github.com/dw-0/kiauh.git)
   ./kiauh/kiauh.sh
