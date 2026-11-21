
[中文](./README.md)
# JetKVM Community
JetKVM (China Supply Chain Edition)  is a lightweight IP KVM operation and maintenance tool，with cost-effective, open-source KVM-over-IP device engineered for reliable remote computer/server management. It allows remote access to a target device’s display and simulates HID input over the network, enabling contactless operation and management of development boards, PCs, and servers. The product delivers stable, low-latency video capture and remote control, making it well-suited for scenarios such as remote computer management and server maintenance. The software is based on a secondary development of  jetkvm/kvm

## Features
* **Micro SD card support**: Used for software boot settings or storage expansion
* **USB multifunction configuration**: Supports emulating a USB sound card or MTP device. Files in the shared MTP directory can be uploaded or downloaded via HTTP
* **Serial port control**: Connects to the serial port of the controlled device for control and debugging
* **IO level configuration**: Controls expansion IO output (high/low level)
* **1.54-inch touchscreen**: Displays IP address, connection status, and system runtime status
* **Multiple remote access methods**: Remote management via WebRTC through cross-network connections or FRP reverse proxy

## Compilation
* Compile frontend only
  ```bash
  make frontend
  ```
* Compile backend only
  ```bash
  make build_dev
  ```
* Full compilation
  ```bash
  make build_release
  ```
* Compile to generate **bin/kvm_app**, then upload the file to JetKVM via SSH or MTP, replacing **/userdata/picokvm/bin/kvm_app**

## Detailed Usage Instructions

