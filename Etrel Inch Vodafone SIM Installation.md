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
2. Search for `Network Connections` and select `View Network Connections`

![IP Network Connections](<Files/Etrel Inch Firmware Update Procedure/ip-network-connections.gif>)
***
3. Double click on `Ethernet`

![IP Network Adapters](<Files/Etrel Inch Firmware Update Procedure/ip-adapters.png>)
***
4. Select `Internet Protocol Version 4 (TCP/IPv4)` then click `Properties`

![IP IPv4](<Files/Etrel Inch Firmware Update Procedure/ip-ipv4.png>)
***
5. Set the following settings then click `Ok`

* **IP Address:** ```192.168.1.33```
* **Subnet Mask:** ```255.255.255.0```

![IP Settings](<Files/Etrel Inch Firmware Update Procedure/ip-settings.png>)
***

## Install SIM

* Insert the SIM card into the SIM tray. The SIM tray is located on the inside of the charger's service door. See photos for reference.

> [!CAUTION]
> Inserting the SIM card in the wrong orientation could cause damage to the charger. Observe photos for the correct orientation.

| ![ SIM Slot ](< Files/Etrel Inch Vodafone SIM Installation/sim-slot.jpg >) | ![ SIM Slot Orientation Front ](< Files/Etrel Inch Vodafone SIM Installation/sim-slot-front.jpg >) | ![ SIM Slot Orientation Back ](< Files/Etrel Inch Vodafone SIM Installation/sim-slot-back.jpg >) | ![ SIM Slot Orientation Back ](< Files/Etrel Inch Vodafone SIM Installation/sim-slot-inserted.jpg > ) |
|----------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------|


## Configure Charger
1. Plug the ethernet cable into your laptop and the charger

The ethernet port on the charger is located behind the access door in the top right hand corner.
***
2. Navigate to the Charger Web GUI

Type the IP address of the charger into your web browser. Make sure to include the `http://` before the IP address.

The charger IP address can be found by opening the service menu (hold down the white button on the inside of the service door until you hear a beep) on the charger and then opening the `1. Communications` menu. The IP address is at the top.

![Service Menu IP](<Files/Etrel Inch Vodafone SIM Installation/service-menu-ip.jpg>)

> [!NOTE]
> If you see a IP address starting in `169.xxx.xx.xx` set your network adapter back to DHCP. [This involves reverting the changes peformed in this section](#configure-windows-network-adapter). Call Thundergrid's Network Operations team on `0800 387 877` for help.

The default IP address is `192.168.1.250`.

Full Example ▶️ `http://192.168.1.250`

![Charger Access](<Files/Etrel Inch Firmware Update Procedure/charger-access.gif>)
***
3. Login to the charger

Use the default password unless otherwise specified

**Username:** `root@etrel.com`

**Password:** `toor`

![Charger Login Screen](<Files/Etrel Inch Firmware Update Procedure/charger-login-screen.png>)
***
4. Configure APN

Go to `Configuration` > `Connectivity` > `GSM connectivity`

Set the `APN` field to: `tg.lte.apac.prod`

Click `Save`

![Set APN](<Files/Etrel Inch Vodafone SIM Installation/set-apn.gif>)

***
5. Reboot charger

Go to `Diagnostics` > `Restart device` > `Yes`

![Reboot Charger](<Files/Etrel Inch Vodafone SIM Installation/reboot.gif>)

***
6. Login and confirm connectivity

Login to the charger and open the connectivity status menu to confirm connectivity. Allow the charger up to 5 minutes to connect after initial startup. Verify that the charger is reporting as `Connected`.

![Connected SIM](<Files/Etrel Inch Vodafone SIM Installation/connected-sim.gif>)

> [!NOTE]
> If the charger reports an error message and the `SIM status` is `SIM Not Present` this may be because of a faulty SIM tray. Verify the SIM card has been inserted in the correct orientation (rebooting the charger after any changes is required for detection). Call Thundergrid's Network Operations team on `0800 387 877` for help.

***

Call Thundergrid's Network Operations team on `0800 387 877` for help, to confirm connectivity & a successful installation.