### Firmware & Control Interface for Nano Light 2 Astronomical Equatorial Mount

**Nano Light** is an open-source DIY equatorial mount project that originated from [here](https://www.bilibili.com/video/BV1gi4y1R7HK?spm_id_from=333.337.search-card.all.click).

This repository contains the code needed for Nano Light **version 2**, including the firmware for the control board and the webpage for mobile control.

---

### Software

#### Overview

The project is divided into two parts:
1. The server flashed into the ESP32, found in the `nano_core` folder.
2. The webpage for display, found in the `nano_view` folder.

The following instructions guide you through the installation and flashing process.

#### Nano View

This is the webpage for mobile control, developed using the React framework. It depends on Node.js and npm.

Two installation options are provided; if no modifications are necessary, the second option is recommended.

- **Manual Build**
    ```bash
    # Install dependencies
    # Navigate to the project directory
    cd nano_view
    # Build
    npm run build
    ```
    The build process will automatically copy the generated files to the `/nano_core/data` directory.
  
- **Prebuilt Package [Recommended]**  
    Download the prebuilt package and manually extract it into the `/nano_core/data` directory.

#### Nano Core

This part includes motor control for the equatorial mount and the server for the control webpage. Complete the `nano_view` section first before proceeding.

Steps:
1. **Environment Setup**
    - Download and install VS Code: [Reference](https://code.visualstudio.com/)
    - Install PlatformIO: [Reference](https://platformio.org/install/ide?install=vscode)
2. Open the project.
3. Build the project.
4. Upload the firmware.
5. Build the file system.
6. Upload the file system.

---

### Open Source License

All files are released under the CC BY-SA license.
