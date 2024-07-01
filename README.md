# Bee-Sync-Flasher



# Firmware Flashing Tool

This repository provides a tool and instructions to flash Z-Stack firmware onto your device.

## Download the Zip File

Download the latest release of the tool from the [Releases page](https://github.com/YOUR_USERNAME/YOUR_REPOSITORY/releases).

## Create a Batch Script

Create a batch script (`flash_firmware.bat`) with the following content:  
*Note: Save the batch file in the same directory where you extracted the zip file.  

```batch
@echo off
set /p COM_PORT="Enter COM port (e.g., COM8): "

flasher_cc2538.exe -p %COM_PORT% -ewv [ENTER YOUR FIRMWARE PATH]
```

## Run the Batch Script

1.Open a Command Prompt window.  
2.Navigate to the directory where you saved the batch script and the extracted files.  
3.Run the batch script by typing flash_firmware.bat and press Enter.  
4.When prompted, enter the COM port (e.g., COM8).  
5.The firmware flashing process will start.  
  
Note: The firmware file to flash must be the latest version.  
  
## Lated Firmware Files Source
-For coordinator firmware, visit [Coordinator Firmware](https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0/bin) and select the appropriate Launchpad_coordinator file.  
-For router firmware, visit [Router Firmware](https://github.com/Koenkk/Z-Stack-firmware/tree/master/router/Z-Stack_3.x.0/bin)and select the appropriate Launchpad_router file.  
*Ensure you download the correct firmware file and place it in the same directory as the batch script.
