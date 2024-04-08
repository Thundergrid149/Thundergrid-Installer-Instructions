# Configure Windows Network Adapter

# Firmware Update Path
The firmware must be updated in a specific order. Please apply the ```system``` firmware before the ```app``` firmware.
```mermaid
flowchart LR

A[5.X]-->|System|B
B[5.0.5]-->|App|C
C[5.4]
```
***
## Download the latest firmware updates

[Download Firmware (App 5.4)](https://etrelchargingsolutions.atlassian.net/wiki/download/attachments/3885269020/inch-app-5.4.armv7.itb?api=v2)

[Download Firmware (System 5.0.5)](https://etrelchargingsolutions.atlassian.net/wiki/download/attachments/3641540644/inch-system-5.0.5.armv7.itb?api=v2)
# Firmware Update
1. Navigate to the Charger Web GUI

Type the IP address of the charger into you web browser. Make sure to include the ```http://``` before the IP address. Example ▶️ ```http://192.168.1.250```

The charger IP address can be found by opening the service menu on the charger then opening the ```1. Communications``` menu.

The default IP address is ```192.168.1.250```
***
2. Login to the charger

Use the default password unless otherwise specified

**Username:** ```root@etrel.com```

**Password:** ```toor```
***
3. Upload charger firmware

Open the charger menu in the top left corner of the screen. Click the ```diagnostics``` section. Select ```Upload Firmware```. Select the firmware you downloaded earlier from your computer.

> [!NOTE]
> The firmware update usually takes 2-3 minutes but sometimes can be longer
***
4. Repeat steps 1 to 3 until at the latest version

# Charger Service Menu
The charger service menu can be opened by holding down the white button inside the charger access panel for 2-3 seconds. The charger should make a beep when the menu has been successfully accessed.
