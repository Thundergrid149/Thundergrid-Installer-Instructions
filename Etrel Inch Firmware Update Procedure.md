# Etrel Inch Firmware Update Procedure
Updating the firmware consists of the following two major steps
* Configure your computer's network adapter to allow you to communicate with the charger
* Uploading the firmware update to the charger

## Configure Windows Network Adapter
Below are steps to configure your network adapter on Windows to connect to the charger with an ethernet cable.

1. In Windows, open the control panel

![IP Control Panel](https://github.com/Thundergrid149/Thundergrid-Installer-Instructions/blob/e2b65bca289407feab340a1447948859df022682/Files/Etrel%20Inch%20Firmware%20Update%20Procedure/ip-control-panel.gif)
***
2. Search for ```Network Connections``` and select ```View Network Connections```

![IP Network Connections](https://github.com/Thundergrid149/Thundergrid-Installer-Instructions/blob/e2b65bca289407feab340a1447948859df022682/Files/Etrel%20Inch%20Firmware%20Update%20Procedure/ip-network-connections.gif)
***
3. Double click on ```Etherent```

![IP Network Adapters](https://github.com/Thundergrid149/Thundergrid-Installer-Instructions/blob/e2b65bca289407feab340a1447948859df022682/Files/Etrel%20Inch%20Firmware%20Update%20Procedure/ip-adapters.png)
***
4. Select ```Internet Protocol Version 4 (TCP/IPv4)``` then click ```Properties```

![IP IPv4](https://github.com/Thundergrid149/Thundergrid-Installer-Instructions/blob/a3c3ff82a1d33f07f6e4f6c8291bc4b6ebb006fb/Files/Etrel%20Inch%20Firmware%20Update%20Procedure/ip-ipv4.png)
***
5. Set the following settings then click ```Ok```

* **IP Address:** ```192.168.1.33```
* **Subnet Mask:** ```255.255.255.0```

![IP Settings](https://github.com/Thundergrid149/Thundergrid-Installer-Instructions/blob/a3c3ff82a1d33f07f6e4f6c8291bc4b6ebb006fb/Files/Etrel%20Inch%20Firmware%20Update%20Procedure/ip-settings.png)
***

## Firmware Update Path
The firmware must be updated in a specific order. Please apply the ```system``` firmware before the ```app``` firmware.

If the charger is on a version starting with `4.0` you will have to update to `5.0` first. [5.0 Download](https://landisgyr-evsolutions.atlassian.net/wiki/spaces/Home/pages/3221094430/5.0)
```mermaid
flowchart LR

A[5.X]-->| System |B
B[5.0.5]-->| App |C
C[5.4]
```
***
## Download the latest firmware updates

[Download Firmware (App 5.4)](https://etrelchargingsolutions.atlassian.net/wiki/download/attachments/3885269020/inch-app-5.4.armv7.itb?api=v2)

[Download Firmware (System 5.0.5)](https://etrelchargingsolutions.atlassian.net/wiki/download/attachments/3641540644/inch-system-5.0.5.armv7.itb?api=v2)

## Perform Firmware Update
1. Navigate to the Charger Web GUI

Type the IP address of the charger into your web browser. Make sure to include the ```http://``` before the IP address. Example ▶️ ```http://192.168.1.250```

The charger IP address can be found by opening the service menu on the charger and then opening the ```1. Communications``` menu.

The default IP address is ```192.168.1.250```

![Charger Access](https://github.com/Thundergrid149/Thundergrid-Installer-Instructions/blob/cb295b992cc7a42101c873787e552edf317dd2b2/Files/Etrel%20Inch%20Firmware%20Update%20Procedure/charger-access.gif)
***
2. Login to the charger

Use the default password unless otherwise specified

**Username:** ```root@etrel.com```

**Password:** ```toor```

![Charger Login Screen](https://github.com/Thundergrid149/Thundergrid-Installer-Instructions/blob/cb295b992cc7a42101c873787e552edf317dd2b2/Files/Etrel%20Inch%20Firmware%20Update%20Procedure/charger-login-screen.png)
***
3. Upload charger firmware

Open the charger menu in the top left corner of the screen. Click the ```diagnostics``` section. Select ```Upload Firmware```. Select the firmware you downloaded earlier from your computer.

![Charger Firmware Upload](https://github.com/Thundergrid149/Thundergrid-Installer-Instructions/blob/cb295b992cc7a42101c873787e552edf317dd2b2/Files/Etrel%20Inch%20Firmware%20Update%20Procedure/charger-firmware-upload.gif)

> [!NOTE]
> The firmware update usually takes 2-3 minutes but sometimes can be longer
***
4. Repeat steps 1 to 3 until at the latest version

## Charger Service Menu
The charger service menu can be opened by holding down the white button inside the charger access panel for 2-3 seconds. The charger should make a beep when the menu has been successfully accessed.
