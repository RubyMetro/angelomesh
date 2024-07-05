---
layout: page
title: getting started
---

---
# Hey There!
We are glad to see that you are interested in building a meshtastic node for your own. Meshtastic nodes help everyone around to communicate with each other, even if you don't see it.

This guide will walk you through what you should consider when purchasing your first meshtastic compatible device (as well as a few popular options,) and a step by step guide for building your very own RAK4631/4630 meshtastic radio.

---

## Selecting a radio
When choosing your very first radio, there are a lot of option to choose from depending on your needs. If you want a radio that works out of the box, you may go with a radio like the LILYGO T-Echo, or rather if you want a radio to work as an MQTT gateway, you may get a T-Beam. Below we have listed some of the most common radios and how they differ, sorted by microcontroller.

- ESP32
    - LILYGO TTGO T-Beam, great if you want to be able to access your radio over WiFi.
    - Heltec V3, cheap, easy to set up, and readily available.
- nRF52
    - LILYGO TTGO T-Echo, comes with an e-ink display and is ready to go out of the box
    - RAK 4631/4630 module for WisBlock boards, infinitely customizable and relatively cheap, very low power consumption and thus great for stationary nodes.

---
## Flashing the firmware
<p class="message">
  WARNING: before plugging your radio into power you MUST make sure that the antennas are attached, running some boards without antennas may damage the microcontroller.
</p>

Before getting started with flashing the firmware, make sure to grab a cable that supports data transfer. Some usb cables are only capable of charging. The process for flashing the [firmware](https://meshtastic.org/downloads/) depends on what model radio you have, this guide will focus on the RAK4631/4630 (however this should work for most nRF52 based devices.)

For flashing the RAK4631/4630, there are two main ways of doing so, **drag and drop** and **OTA.** We will be going over both in this guide, however it is reccomended that you learn how to upgrade your firmware via OTA so that you are able to do so easily if you ever have a node that is in a hard or impossible to reach position.

### Drag and drop
1. Start by plugging your device into your computer with a USB data cable.
2. Download the latest [firmware](https://meshtastic.org/downloads/) from Meshtastic.
3. Double click the reset button on your device. This will put it into bootloader mode and allow the device to show up as a drive on your computer.
4. Ensure a drive has mounted on your machine.
5. Open this drive, and copy the appropriate firmware file (in this case the file should be named **firmware-rak4631-CURRENT-VERSION.uf2**)
6. Once the file has finished copying onto the drive, your radio will reboot and flash the firmware. You are now ready to pair your radio with your phone/computer

### OTA
<p class="message">
  Note: As of this writing, the current Android release of the nRF DFU app is not compatible with meshtastic firmware.
</p>

- Android instructions
    1. Download the more advanced nRF Connect App (v 4.24.3), available [here.](https://github.com/NordicSemiconductor/Android-nRF-Connect/releases/tag/v4.24.3)
    2. Download the latest [firmware](https://meshtastic.org/downloads/) from Meshtastic.
    3. Open the nRF Connect App and select **Connect** on your radio from the **Scanner** tab
    4. Select the DFU icon from the top-right of the screen
    5. Select the device firmware file, will most likely look like **firmware-rak4631-CURRENT-VERSION-ota.zip**, do not unzip this file.
    6. The update will begin.

- iOS/iPadOS/macOS instructions
    1. Download the nRF Device Firmware Update App on the App Store
    2. Download the latest [firmware](https://meshtastic.org/downloads/) from Meshtastic.
    3. Open the nRF DFU App and select the correct device firmware file, will most likely look like **firmware-rak4631-CURRENT-VERSION-ota.zip**, do not unzip this file.
    4. Connect your device
    5. Upload the firmware.

---
## Connecting your radio to your phone or computer
To connect your radio to your phone or computer you will need to download the meshtastic app, which is available for Android, iOS, and macOS. This guide will be focusing on the iOS version of the app but the process is mostly the same.

To start, you will want to download and then open the Meshtastic app.
<img src="/Assets/gs1.PNG" width="200"/>
Next, you will want to select your radio. It will most likely be named something like "Meshtastic_81d3." If you are unable to find your device, try moving away from other Meshtastic devices in the area. It will ask for a pin, and the default is 123456. This can be changed later in settings.
<img src="/Assets/gs2.PNG" width="200"/>
After your pin has been entered, your radio will connect and you should see something like this:
<img src="/Assets/gs3.PNG" width="200"/>

The above steps work the exact same way on macOS and iPadOS as well. Alternatively, if you would like to use your radio over a USB serial connection instead, you can connect it directly to your computer and go to [the meshtastic web client.](https://client.meshtastic.org)

<p class="message">
  Note: If using a browser such as Safari or Firefox, you will only be able to access your radio if it is accessible through an IP address or HTTP, for bluetooth and serial connections, Chrome is required.
</p>

---
## Conclusion
Congratulations! You just set up your first Meshtastic enabled radio. You are now helping the resiliance of the mesh network here in San Angelo.