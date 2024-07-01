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

Save the file in the same directory where you extracted the zip file.

Run the Batch Script
Open a Command Prompt window.
Navigate to the directory where you saved the batch script and the extracted files.
Run the batch script by typing flash_firmware.bat and press Enter.
When prompted, enter the COM port (e.g., COM8).
The firmware flashing process will start.
Note: The firmware file to flash must be the latest version.

Firmware Files
For coordinator firmware, visit Coordinator Firmware and select the appropriate Launchpad_coordinator file.
For router firmware, visit Router Firmware and select the appropriate Launchpad_router file.
Ensure you download the correct firmware file and place it in the same directory as the batch script.

Additional Resources
For more information about the flashing tool, refer to the flashing tool documentation.
For driver installation, visit Silicon Labs USB to UART Bridge VCP Drivers.
Feel free to open an issue if you encounter any problems or have questions.
