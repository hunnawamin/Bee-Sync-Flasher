# Bee-Sync-Flasher
# Firmware Flashing Tool

This repository provides a tool and instructions to flash Z-Stack firmware onto your device.

## Download the Zip File

Download the latest release of the tool from the [Bee-Sync-Flasher](https://github.com/hunnawamin/Bee-Sync-Flasher/blob/main/Bee-Sync-Flasher.rar).
 {ดาวน์โหลดซิปไฟล์นี้}
## Create a Batch Script

Edit the batch script (`Flash-CE-coordinator.bat`) with your firmware path which is (.hex) file:  
*Note: Save the batch file in the same directory where you extracted the zip file.  
 {แก้ไข batch script โดยใส่ Firmware Path ของไฟล์ .hex ตามนี้}
```batch
@echo off
set /p COM_PORT="Enter COM port (e.g., COM8): "

flasher_cc2538.exe -p %COM_PORT% -ewv [ENTER YOUR FIRMWARE PATH]

if "%errorlevel%"=="0" cls &Echo Success.
timeout /t 3
if "%errorlevel%"=="1" cls &Echo Fail
timeout /t 3

```

## Run the Batch Script

0. (Need to Unpack the package) Press and hold the Flash button about 2 Seconds and Connect your device through USB.
1.Double-click to Flash-CE-coordinator.bat file.  
2.When prompted, enter the COM port (e.g., COM8).  
3.The firmware flashing process will start.  
  
Note: The firmware file to flash must be the latest version.  
  
## To Update and/or Check The Lated Firmware Files Source
-For coordinator firmware, visit [Coordinator Firmware](https://github.com/Koenkk/Z-Stack-firmware/tree/master/coordinator/Z-Stack_3.x.0/bin) and select the Launchpad_coordinator file.  
-For router firmware, visit [Router Firmware](https://github.com/Koenkk/Z-Stack-firmware/tree/master/router/Z-Stack_3.x.0/bin)and select the Launchpad_router file.  
*Ensure you download the correct firmware file and place it in the same directory as the batch script.
