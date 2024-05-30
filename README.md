# BlueHack
A tool which perform deauthentication attack on bluetooth devices.

# Setup
Make sure the latest python and pip3 is installed on your system (Windows/Linux/MacOS).

# Install and Run
## 1. Run the following command to start terminal in root :
   ```
   sudo su
   hciconfig
   hciconfig hci0 up
   service bluetooth restart
   git clone https://github.com/3xpell14rmu5/BlueHack-.git
   cd BlueHack-
   python3 BlueHack.py
   ```
# For Better Results
- Use a Bluetooth Adapter for better results of the tool.
- Make sure that Bluetooth Adapter supports `HCI` mode.
- **TP-Link UB400 USB Bluetooth Adapter** is one of the Bluetooth Adapter.
- To check Bluetooth Adapter supports HCI mode or not, there are two ways :
  1. Type `lsusb` command after connecting adapter to the system.
     - It show the `(HCI Mode)` at the end of the adapter name means it supports HCI mode.
  2. Type `hciconfig hciX up`.
     - If it is up then it supports HCI mode, otherwise not.

# Warning
- Some cheap Bluetooth Adapters show that it supports HCI mode but it does not work.
- Some cheap Bluetooth Adapters works on only one OS but not on other OS.
- Some cheap Bluetooth Adapters does not support Linux.

# Some Comman Errors
1. `Host is down` - The bluetooth device is connected to the device.
2. `Connection timed out` - The bluetooth device is powered off.
3. `Connection reset by peer` - The device bluetooth is turned off.

# In case...
If the tool is not working, then type the following command to restart bluetooth services :
```
sudo service bluetooth restart
```
