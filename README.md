# ADB-GUI
UI wrapper around ADB to make life easier for Android Developer and QA

[Install](https://github.com/yapplications/ADB-GUI/blob/master/README.md#install) </br>
[Abilities](https://github.com/yapplications/ADB-GUI/blob/master/README.md#abilities) </br>
[Use Cases](https://github.com/yapplications/ADB-GUI/blob/master/README.md#use-cases) </br>
[Known Isseus](https://github.com/yapplications/ADB-GUI/blob/master/README.md#known-issues) </br>

## Install:

* You should have Java and adb (comes with android studio) installed.

1. Dowload: 

2. Unzip to a path **without spaces**  

3. MAC: give running permission to: ADB-GUI-Tool.jar

4. Run: ADB-GUI-Tool.jar (Double press from finder / explorer or run: `java -jar ADB-GUI-Tool.jar` from terminal)

5. On first run: change 'adb path' in preference screen to point to your local adb

## Abilities:

The app devided into Device Panel 7 Tabs and status line

#### Status line:

Appears at the bottom, most of the commands will update it.

  * Black color text: command is running
  * Green color text: command executed succesfully
  * Red   color text: command failed

Some commands will appear green result even if the command failed

#### Device Panel:

1. Device selection: all device commands that you will execute will be executed on the device you select here

2. Connect device via WiFi: click in order to start working via WiFi
  * Device should be on the same network as the pc
  * After pressed there should be an extra device in the list and you can disconnect it from usb.
  * Connection will be lost if adb / device restarts

3. Take snapshot: opens an 'device view' screen
  * Screen will be updated by itself
  * Press 'Save' to save a snapshot
  * You can save as many snapshots as you like in one session

4. Send quick text to device: enter the text you want to send and press enter

5. Change emulator date: opens a dilog for changing emulator time
..* Works only on emulators
..* Will also disable the auto date / time zone update
..* If you move to the clock extensively it can jump back

6. Open developer settings on the device

7. Open app directory: open the directory where all the files stored on your pc

#### Tabs

1. Batch command

2. Applications

3. APKs

4. Intent / broadcasts

5. Log / Exceptions

6. Terminal

7. Preference


## Use Cases:

## Known Issues

1. Unothorized device: some times the adb devices command will retrive one of the devices as unothorized in this case you should:
  * Press "Kill ADB"
  * Open terminal / command line and write "adb devices" (Running this command from the App not working for some reason)
  * Press "Start monitoring" to get the device list back

2. Some of the functions will not work if the app is placed in path with spaces