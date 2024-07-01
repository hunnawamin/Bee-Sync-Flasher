# Bee-Sync-Flasher



# Firmware Flashing Tool

This repository provides a tool and instructions to flash Z-Stack firmware onto your device.

## Download the Zip File

Download the latest release of the tool from the [Releases page](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY/releases).

## Create a Batch Script

Create a batch script (`flash_firmware.bat`) with the following content:

```batch
@echo off
set /p COM_PORT="Enter COM port (e.g., COM8): "

flasher_cc2538.exe -p %COM_PORT% -ewv [ENTER YOUR FIRMWARE PATH]
