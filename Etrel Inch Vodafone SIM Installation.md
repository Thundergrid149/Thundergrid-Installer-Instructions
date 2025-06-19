# Etrel Inch Vodafone SIM Installation Procedure
Installing the Vodafone SIM consists of the following three major steps
* Configure your computer's network adapter to allow you to communicate with the charger
* Install the SIM in the charger
* Configure the charger and confirm connectivity

> [!IMPORTANT]
> You will need an ethernet cable and laptop to complete this job

## Configure Windows Network Adapter
Below are steps to configure your network adapter on Windows to connect to the charger with an ethernet cable.

1. In Windows, open the control panel

![IP Control Panel](<Files/Etrel Inch Firmware Update Procedure/ip-control-panel.gif>)
***
2. Search for ```Network Connections``` and select ```View Network Connections```

![IP Network Connections](<Files/Etrel Inch Firmware Update Procedure/ip-network-connections.gif>)
***
3. Double click on ```Etherent```

![IP Network Adapters](<Files/Etrel Inch Firmware Update Procedure/ip-adapters.png>)
***
4. Select ```Internet Protocol Version 4 (TCP/IPv4)``` then click ```Properties```

![IP IPv4](<Files/Etrel Inch Firmware Update Procedure/ip-ipv4.png>)
***
5. Set the following settings then click ```Ok```

* **IP Address:** ```192.168.1.33```
* **Subnet Mask:** ```255.255.255.0```

![IP Settings](<Files/Etrel Inch Firmware Update Procedure/ip-settings.png>)
***

## Install SIM

* Insert SIM card

## Configure Charger
1. Plug the ethernet cable into your laptop and the charger

The ethernet port on the charger is located behind the access door in the top right hand corner.
***
2. Navigate to the Charger Web GUI

Type the IP address of the charger into your web browser. Make sure to include the `http://` before the IP address. Example ▶️ `http://192.168.1.250`

The charger IP address can be found by opening the service menu on the charger and then opening the `1. Communications` menu.

The default IP address is `192.168.1.250`

![Charger Access](<Files/Etrel Inch Firmware Update Procedure/charger-access.gif>)
***
3. Login to the charger

Use the default password unless otherwise specified

**Username:** `root@etrel.com`

**Password:** `toor`

![Charger Login Screen](<Files/Etrel Inch Firmware Update Procedure/charger-login-screen.png>)
***
4. Configure APN

`APN`: `tg.lte.apac.prod`

clear username and PIN -> confirm this

***
5. Reboot charger

Add Gif

***
6. Login and confirm connectivity

Add Gif