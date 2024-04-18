# Instructions for Installing Thundergrid LtAP Mini
## Post Installation
> [!IMPORTANT]
> Please take photos of the unit installed and its location. Email these to ```photos@thundergrid.net```

## Positioning
* When mounting outside, aim to have the device out of access from the public and or at a height that is only reachable with a ladder. This is for security and theft prevention.
* When mounting outside, look to place it under an eave to minimise exposure to the elements.
* Please avoid placing it inside metal cabinets as this will lead to poor mobile reception.
* Thundergrid has minimum acceptable reception parameters, make sure the location of the device will achieve this. Please feel free to contact us for more information and support regarding this.

## Mounting
![ltap](https://github.com/Thundergrid149/Thundergrid-Installer-Instructions/blob/030dbc3b237191de3b219814e3e959084cd523d0/Files/ltap-mini-mounting.png)
1. It is possible to attach the device to a wall, using the provided screw holes on the sides of the unit. The device should be mounted in a way that the cable openings are pointing downward as shown in the picture.
2. The ports are protected with a small door, that is held in place with one screw. Use the Philips PH2 screwdriver to access the ports.
3. The door has cut-out places for all available ports, but please only break out the openings that you will use. The device can be used both indoors and outdoors. The IP rating scale for this device is IP54.

## Powering
Powering the device over etherent is the prefered method. The adapater for this is included in the box. This allows you to put the device up to 100 meters away (ethernet cable limit) from the rest of the communcations equipment. The power consumption under maximum load with attachments can reach 9 W.

**Ethernet port accepts passive and 802.3af/at Power over Ethernet 8-57 V DC (compensate for loss on cable, so more than 12 V recommended).**

Connecting to a PoE Adapter:
1. Connect the Ethernet cable from the LtAP Mini to the "Data+Power" (PoE+DATA) port of the PoE adapter.
2. Plug the male end of the PoE adapter into the switch (LAN).
3. Connect the power cord to the adapter, and then plug the power cord into a power outlet.
4. The device should have at least two green LEDs light up if all done correctly

> [!TIP]
> If you have a long etherent run to the LtAP. You can try first plugging in a smaller cable that you know to be working to make sure the PoE injector is configured correctly.

### Powering the PoE Adapter
Both of the following options are acceptable and are included in the box. Choose which ever works better in your specific installation.
1. DC power supply (AC electrical socket).
2. Cable DC with striped 2*24 AWG Tin 8 mm, length 0.35 m.

## Mikrotik Official Information
[https://help.mikrotik.com/docs/display/UM/LtAP+mini](https://help.mikrotik.com/docs/display/UM/LtAP+mini)
