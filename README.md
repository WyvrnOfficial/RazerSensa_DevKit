## Table of Contents
1. [Drivers Update](#drivers-update)
    1. [Kraken Firmware Update](#kraken-firmware-update)
    2. [Razer Sensa devices libraries](#razer-sensa-devices-libraries)
2. [Apps](#apps)
    1. [Mech Warrior 5 Mod](#mech-warrior-5-mod)
    2. [Tech Demo](#tech-demo) 

---

## 1. Drivers Update <a name="drivers-update"></a>

### 1.1. Kraken Firmware Update <a name="kraken-firmware-update"></a> (Location: Drivers\Kraken)

- Plug the Razer Kraken Hypersense device into a USB port of your PC.
- Open the folder `Drivers\Kristal - FactoryFWUKrystalT2STM32_v1.02.03_20211111`. Launch the executable `FactoryFWUKrystalT2STM32.exe`.
- Click on the `Select STM FW` button. A file input popup should appear for bin file.
- Select the Firmware `Jaycee_HapticFW_V1.2.5.9` bin file and open it. The software window should update itself to display the selected file path.
- Click on the `Update STM FW` button. Wait until the loading bar indicates 100%.
- You can close the software, your device firmware is now updated.

![KrakenFW1](Documentation\Images\KrakenFW1.png)
![KrakenFW2](Documentation\Images\KrakenFW2.png)

### 1.2. Razer Sensa devices libraries <a name="razer-sensa-devices-libraries"></a> (Location: Drivers)

- Launch `Install_RzInterHaptics_Inbox_1.0.4.1.exe` to install the Razer Sensa device libraries.

## 2. Apps <a name="apps"></a>

### 2.1. Mech Warrior 5 Mod <a name="mech-warrior-5-mod"></a> (Location: MechWarrior5)

- Copy the folder `RzInterhaptics` from `MechWarrior5\HapticEngine\V2.0.1` to `C:\Program Files (x86)\Interhaptics\` (contains Clipboard Haptic Engine and custom haptic effects).
- Copy the contents of `MechWarrior5` to `C:\Program Files\Epic Games\MW5Mercs\MW5Mercs\Mods`. If the `Mods` folder does not exist, you must create it. A complete guide with pictures can be found inside the `MechWarrior5` folder: `Mod_setup.pdf`.

### 2.2. Tech Demo <a name="tech-demo"></a>
(Empty for now)

[Back to Table of Contents](#table-of-contents)
