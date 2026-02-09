# Background:

This guide outlines the steps required to configure your development environment for the **ESP32-S3** using the Arduino IDE. You should be able to complete all steps until Section 5 without access to the ESP32-S3.

## ESP32-S3 Setup

---

### 1. Install Arduino IDE
Download and install the latest version of the **Arduino IDE** from the official [Arduino website](https://www.arduino.cc/en/software). Make sure you select the correct Windows / MacOS configuration.

### 2. Configure Board Manager URL
To enable support for ESP32 boards on an Arduino IDE, you must point the IDE to the correct package repository.
* Open Arduino IDE.
* Go to **File > Preferences**.
* Locate the **Additional Boards Manager URLs** field and paste the following link:
  `https://dl.espressif.com/dl/package_esp32_index.json`
* Click **OK**.

### 3. Install ESP32 Core
* Navigate to **Tools > Board > Boards Manager...**
* In the search bar, type **esp32**.
* Find the package by **Espressif Systems** and click **Install**.

### 4. Select the Board Module
Once the installation is complete, you need to target the specific hardware:
* Go to **Tools > Board > esp32**.
* Select **ESP32S3 Dev Module** from the list.

### 5. Port Selection & Verification
Ensure the IDE is communicating with your hardware over the correct serial port.
* Connect your ESP32-S3 to your computer via USB.
* Go to **Tools > Port** and select the active port (e.g., `COM12`).
* **Note:** If you are unsure which port is active, check your **Device Manager** under "Ports (COM & LPT)" to identify the device.

### 6. Upload and Flash: 
* Open a sketch from **File > Examples**. To upload the code, click the **Right Arrow (Upload)** button on the top-left of the IDE. 
* Note that you must flash the code every time you make changes to the program to update the ESP32. 
---
