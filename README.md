## Table of Contents
1. [Drivers Update](#drivers-update)
    1. [Razer Synapse 3 Setup](#razer-synapse)
    2. [Razer Kraken Firmware Update](#kraken-firmware-update)
    3. [Razer Sensa Devices Libraries](#razer-sensa-devices-libraries)
    4. [Esther Device Setup](#esther-device-setup)
2. [Apps](#apps)
    1. [Synesthesia App - Hogwarts Legacy](#synesthesia-app)
    2. [Tech Demo](#tech-demo) 
    3. [Mech Warrior 5 Mod](#mech-warrior-5-mod)

---

The Razer Sensa DevKit consists of the following hardware devices and software suite:
- Hardware:
  - Razer Kishi Ultra game controller (retail unit)
  - Razer Kraken headphones (retail unit; needs a firmware update)
  - Razer Esther (pre-production unit)
- Drivers/Firmware:
	- Razer Synapse 3
	- Razer Sensa device drivers
	- Razer Kraken custom firmware
- Demos
  - Hogwarts Legacy PC Version
  - Tech Demo
  - Mech Warrior 5 Mod 
  

## 1. Drivers Update <a name="drivers-update"></a>

### 1.1. Razer Synapse 3 Setup <a name="razer-synapse"></a> (Location: Drivers\Kraken)

- Launch the Razer Synapse 3 setup from the Synapse executable (Location: Drivers\Synapse). The latest version can also be downloaded from this link: https://www.razer.com/synapse-3
- Check the Chroma options during setup.
- After the setup is finished sign in with your Razer Id or create one to get started (or log in as a Guest). 
- If a reboot is required, restart your PC.

![KrakenFW1](Documentation/Images/Razer_Synapse.png)

### 1.2. Kraken Firmware Update <a name="kraken-firmware-update"></a> (Location: Drivers\Kraken)

- Plug the Razer Kraken Hypersense device into a USB port of your PC.
- Open the folder `Drivers\Kristal - FactoryFWUKrystalT2STM32_v1.02.03_20211111`. Launch the executable `FactoryFWUKrystalT2STM32.exe`.
- Click on the `Select STM FW` button. A file input popup should appear for bin file.
- Select the Firmware `Jaycee_HapticFW_V1.2.5.9` bin file and open it. The software window should update itself to display the selected file path.
- Click on the `Update STM FW` button. Wait until the loading bar indicates 100%.
- You can close the software, your device firmware is now updated.

![KrakenFW1](Documentation/Images/KrakenFW1.png)
![KrakenFW2](Documentation/Images/KrakenFW2.png)

### 1.3. Razer Sensa devices libraries <a name="razer-sensa-devices-libraries"></a> (Location: Drivers)

- Launch `Install_RzInterHaptics_Inbox_1.x.x.x.exe` to install the Razer Sensa device libraries. [1.x.x.x - current version of drivers]

### 1.4. Esther Device Setup <a name="esther-device-setup"></a>

#### How to setup Esther

- Put the electrical plug into the socket and attach the cable to Esther.
- Turn on Esther by pushing the power button.
- Plug the USB dongle into your PC.
- LED indicator must be solid green to be connected

![Esther](Documentation/Images/Esther_buttons.png)

#### Button functionalities

- **Power:** Turn ON/OFF the device.
- **Haptic Intensity:** Select general haptic intensity of the device. From level 1 (low) to level 6 (high).
- **Source:** Select between USB dongle (Green) and Bluetooth (Blue, not supported at the current stage).
- **Important Note:** If the light is blinking green, plug the USB dongle in another port. If the light is blue (blinking or solid) that means that the device is in BLuetooth mode and it should be changed by pressing the Source button to the USB 2.4 dongle connection. 

## 2. Apps <a name="apps"></a>

### 2.1 Synesthesia App <a name="synesthesia-app"></a> (Location: Synesthesia)

##### 2.1.1 Overview

The Synesthesia engine integrates the Chroma DLL enabled games with various Razer Sensa haptic devices to provide a synchronized gaming experience that involves dynamic haptic feedback based on in-game events. The DevKit contains an example of the Hogwarts Legacy haptic integration. A complete documentation on Synesthesia can be found at this link: https://www.interhaptics.com/doc/chroma-sensa/#synesthesia 

The Synesthesia apps can be found in the folder `ReleaseConsole`. The engine will be shipped in Synapse when Esther and Kraken V4 will launch.  

##### 2.1. Test Hatics with Hogwarts Legacy PC Version

- Install the PC version of Hogwarts Legacy.
- Plug in the Razer Sensa haptic devices.
- Open Synapse and uncheck `ENABLE THIS APP` from the `CONNECT'->'APPS' section. 
![Hogwarts1](Documentation/Images/Chroma_Connect_Apps.png)
- Launch the Synesthesia app from the Synesthesia/ReleaseConsole folder (as Administrator). 
- Launch the Hogwarts Legacy game.
![Hogwarts2](Documentation/Images/SynesthesiaHogwarts.png)
- Stupefy! 
*Haptics is implemented on all magic spells. If you have not played Hogwarts Legacy, install this save file through this quick guide:
- Boot up the game from your Steam/Epic account. Once it shows the Hogwarts letter, exit out of the game.
- Disable Steam Cloud for the save games of Hogwarts Legacy. Right-click on Hogwarts Legacy (see image below).
![Hogwarts3](Documentation/Images/Hogwarts_Legacy_SteamCloud.png)
- In your file explorer go to `C:\Users\<Your USERNAME>\AppData\Local\Hogwarts Legacy\Saved\SaveGames`
- Make duplicates of all the folders at that location (should be labeled with numbers). 
- Delete the content of the original folder. Unpack HogwartsLegacySaveGame.zip in the now empty folder.

### 2.2. Tech Demo <a name="tech-demo"></a> (Location: TechDemo)
- Close Synesthesia Console
- Decompress the file TechDemo_V[x.x.x].zip in a folder of your choice.
- Launch the TechDemo app from inside the unarchived folder.
- Press Play and enjoy the Razer Sensa Tech Demo.

![TechDemoSettings](Documentation/Images/TechDemoSettings.png)

### 2.3. Mech Warrior 5 Mod <a name="mech-warrior-5-mod"></a> (Location: MechWarrior5)

- Copy the folder `RzInterhaptics` from `MechWarrior5\HapticEngine\V2.0.1` to `C:\Program Files (x86)\Interhaptics\` (contains Clipboard Haptic Engine and custom haptic effects).
- Copy the contents of `MechWarrior5` to `C:\Program Files\Epic Games\MW5Mercs\MW5Mercs\Mods`. If the `Mods` folder does not exist, you must create it. A complete guide with pictures can be found inside the `MechWarrior5` folder: `Mod_setup.pdf`.
- Run ProtoComUnreal.exe from RzInterhaptics\x64\Release.


[Back to Table of Contents](#table-of-contents)
