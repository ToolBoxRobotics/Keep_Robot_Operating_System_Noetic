# Keep_Robot_Operating_System_Noetic

## Install the Arduino IDE on Ubuntu

### Method 1: Use Snap (Recommended for simplicity)

1. Open a terminal.
2. Run the following command to install the Arduino IDE via Snap:
```bash
sudo snap install arduino
```
3. Launch the IDE by searching for "Arduino" in your applications menu or by typing arduino in the terminal. 

### Method 2: Use APT (Quick installation) 

    Open a terminal.
    Update your package list and install the Arduino IDE:
    bash

sudo apt update
sudo apt install arduino

Launch the application by searching for "Arduino" in your applications menu. 

Method 3: Download the AppImage (For the latest version) 

    Go to the official Arduino IDE download page and download the AppImage for your system architecture (e.g., 64-bit).
    Find the downloaded file (it will likely be in your Downloads folder).
    Make the file executable. You can do this in two ways:
        Via the terminal: chmod +x arduino-ide_*.AppImage
        Via the file manager: Right-click the file, select "Properties," go to the "Permissions" tab, and check the box for "Allow executing file as program".
    Double-click the AppImage file to launch the Arduino IDE. 

Final step: Grant serial port access

    After installing via any method, you may need to grant yourself access to the Arduino's serial port.
    Open a terminal and run the following command:
    bash

sudo usermod -a -G dialout $USER

Log out and log back in for the group changes to take effect. 
