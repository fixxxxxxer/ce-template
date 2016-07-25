# Quickstart

Learn about your Helio X20 board as well as how to prepare and set up for basic use

## Setup - What you will need

**Need**
- [Power adapter](https://www.96boards.org/products/accessories/power/)
   - 96Boards specifications requires a 6.5V-18V with 2000mA Power adapter
- [USB Keyboard and Mouse](USBKeyBoardMouse.md)
   - With two USB-A connectors, all 96Boards can be equiped with a full sized keyboard and mouse
- Full size HDMI Cable
   - All 96Boards are equiped with a full sized HDMI connector
- Monitor
   - HDMI capable monitor is recommended

**Optional**
- MicroSD card with adapter
   - For quick and easy switching between operating systems and extra storage
- [Mezzanine Products](../../../MezzanineProducts/README.md)
   - These devices allow you to expand your experience with any 96Boards by adding peripherals and enhancing onboard components
- USB to MicroUSB cable
   - This is needed for serial console interface and fastboot/adb commands
- USB to ethernet adapter and ethernet cable
   - For connecting to a network without using WiFi

***

# Out of the Box

The following subsections should describe how to get started with the Helio X20 using the release build shipped with the boards. The Helio X20 Development Board is ready to use “out of the box” with a pre-installed version of Android.

<img src="http://i.imgur.com/Mdjs6Nx.png" data-canonical-src="http://i.imgur.com/Mdjs6Nx.png" width="250" height="160" />
<img src="http://i.imgur.com/3EleXMR.png" data-canonical-src="http://i.imgur.com/3EleXMR.png" width="250" height="160" />
<img src="http://i.imgur.com/p1N2nDt.png" data-canonical-src="http://i.imgur.com/p1N2nDt.png" width="250" height="160" />

To get started you will need a power supply, an HDMI monitor, a USB keyboard and a USB mouse

## Updating to a new release or change your operating system

If you are already familiar with the Helio X20 board and would like to change out the stock operating system please proceed to one of the following pages:

- [**Downloads page**](../Downloads/README.md): This page lists all Linaro and 3rd party operating systems available for Helio X20
- [**Installation page**](../Installation/README.md): If you already have the images you need, this page has information on how to install the different operating systems onto your Helio X20 board
- [**Board Recovery**](../Installation/BoardRecovery.md)
   - If at any time your board is having unexplainable issues, it is suggested to attempt a board recovery. These instructions will guide you through a succesfull board recovery.
- [**Troubleshooting**](../Troubleshooting/README.md)
   - From bug reports and current issues, to forum access and other useful resources, we want to help you find answers

## Update your system

< Insert system update information >

## Features

|     |     |
|:----|:----|
| SoC | Helio X20   |
| CPU | 2x ARM Cortex-A72 @ 2.1GHz ~ 2.3GHz<br>4x Cortex-A53 @ 1.95GHz<br>4x Cortex-A53 @ 1.4GHz |
| GPU |ARM Mail-T880 GPU operating at up to 800MHz |
| RAM | DDR: 2GB LPDDR3  |
| PMU | HI6553V100|
| Storage |	8GB eMMC5.1 on board storage MicroSD card slot  |
| Ethernet Port | USB2.0 expansion |
| Wireless | Wi-Fi 802.11 a/b/g/n + Bluetooth 4.1  |
| USB | 2 x USB2.0 Host 1 x USB 2.0 OTG  |
| Display | 1 x HDMI 1.4 (Type A - full) 1 x MIPI-DSI HDMI output up to FHD 1080P|
| Video | 1080p@30 fps HD video encoding, supporting 1080p@30 fps HD camera 1080p@30 fps HD video decoding Supports H.264, SVC, MPEG1/2/4, H.263, VC-1, WMV9, DivX, RV8/9/10, AVS, VP8  |
| Audio | HDMI output|
| Camera | One 4-lane MIPI camera serial interface(CSI), one 2-lane MIPI CSI|
| Expansion Interface |40 pin low speed expansion connector: +1.8V, +5V, SYS_DCIN, GND, UART, I2C, SPI, PCM, PWM,GPIO x12 60 pin high speed expansion connector:   SDIO, MIPI_DSI, MIPI_CSI  |
| LED |	1 x WiFi activity LED（Yellow） 1 x BT  activity LED (Blue) 4 x User LEDs (Green)|
| Button  |Power Button ： Button Power on/off & Reset the system|
| Power Source | 8V~18V@3A, Plug specification is inner diameter 1.7mm and outer diameter 4.8mm|
| OS Support |	Android 4.2/Linux |
| Size |	85mm x 55mm  |

**IMPORTANT NOTES**

HDMI EDID display data is used to determine the best display resolution. On monitors and TVs that support 1080p (or 2K) this resolution will be selected. This selected mode will work with most but not all monitors/TVs. See below for further information on what to do if your monitor/TV does not display the UI.
There are limitations on the usage of the USB ports on the Helio X20 Development Board. Please refer to the Hardware section in the document for further information.

## Power Supply

The Helio X20 Development Board requires an external power supply providing 12V at 2A. (The board will also work with 8V or 18V power supplies). It is also possible to power the board from a USB power supply, this is a feature of the MediaTek Helio X20 Development Board. 

The Helio X20 Development Board uses an EIAJ-3 DC Jack with an outer diameter 4.75mm and a 1.7mm barrel, center pin positive. Please do not use EIAJ-2 plug that has an outer diameter 4.0mm and a 1.7mm barrel which fits to the the EIAJ-3 DC jack but it will have weak ground connection because of smaller diameter and makes the board unstable.

## Monitor

A standard monitor or TV supporting at least 640*480 resolution is required. Interlaced operation is not currently supported. The maximum resolutions currently supported are 1920*1080p. Information on selecting the resolution is provided below. 

## Wireless Network

The Helio X20 Development Board includes built-in 2.4GHz IEEE802.11 a/b/g/n WiFi networking. The board also supports the 5GHz band. To use the wireless LAN for the first time (or to switch wireless networks), you should click on the wireless LAN icon from the shortcut menu or through the Wi-Fi option in Settings application. The right hand fifth orange LED will light up indicates wireless network activity. You could configure the network through UI.

## Bluetooth

The Helio X20 Development Board includes built-in Bluetooth 4.1 LE support.

To setup a Bluetooth device open the Bluetooth Manager from the shortcut menu or through the Bluetooth option in Settings application. Open the bluetooth and it will automatically start to search for devices, you could click on “Refresh” to search for devices again. You could try with your bluetooth audio or bluetooth keyboard/mouse.

The right hand sixth blue LED will light up indicates bluetooth activity.

## Audio Device

Bluetooth audio devices are supported on Helio X20 Development Board. Follow normal procedures of connecting a bluetooth device to connect to your board.

NOTE: HDMI audio is also supported in this release.

Once Bluetooth sound sink is connected, you can open the Music player from the Applications UI. Create a playlist from your music files. Supported audio formats are .mp3, .ogg and .wav. You should now be able to play from the Music player.

## File System

Helio X20 Development board comes with 8GB for eMMC size.

## Tri-Cluser Deca-Core

- Two 2.3-2.5GHz A72 core, responsible for showing the highest performance.
- Four 2.0GHz A53 core, responsible for balancing performance and power consumption.
- Four 1.4GHz A53 core, responsible for the low load tasks and power saving.

## Clock

The Helio X20 board does not support a battery powered RTC. System time will be obtained from the network if available. If you are not connecting to a network you will need to manually set the date on each power up.

## System and User LEDs

Each board led has a directory in /sys/class/leds. By default the LEDs use the following triggers:

LED | Trigger
--- | -------
wifi_active | phy0tx (WiFi Tx)
bt_active | hci0tx (Bluetooth Tx)
user_led1 | heartbeat
user_led2 | mmc0 (disk access, eMMC)
user_led3 | mmc1 (disk access, microSD card)
user_led4 | CPU core 0 active(not used)

To change a user LED you can do the following as a root user (using ADB):
```
# echo heartbeat > /sys/class/leds/<led_dir>/trigger      make a LED flash
# cat /sys/class/leds/<led_dir>/trigger                   show triggers
# echo none > /sys/class/leds/<led_dir>/trigger           remove triggers    
# echo 1 > /sys/class/leds/<led_dir>/brightness           turn LED on
# echo 0 > /sys/class/leds/<led_dir>/brightness           turn LED off
```
