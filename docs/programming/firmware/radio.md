# Radio Firmware
--8<-- "incomplete.md"

## Downloading Radio Configuration Utility

!!! note

    If you have downloaded the FRC Game Tools package from NI, this tool should already have been installed. You should not need to download it again unless it's missing.

The FRC Radio Configuration tool is needed to configure the radio. Please see the [documentation](#helpful-links) for the up-to-date download link. After the tool is downloaded, unzip it, and use the EXE file to run the tool. Ensure that the tool is run as an Administrator (it should prompt you to do so if you don't) -- it will not work otherwise.

## Configuring the Radio

!!! info
    This section is not yet completed

<!-- TODO -->

## Troubleshooting
### Radio is not turning on
Ensure that the POE (Power over Ethernet, a.k.a. the orange Ethernet cable) is connected to the bottom (the one next to the barrel power connector), and that the barrel power connector is connected to the VRM (Voltage Regulator Module). For additional details, please see the electrical documentation. <!-- TODO: Update with electrical link once created -->

### What network interface do I use?
If prompted for a network interface (if you choose the wrong one earlier, you can use the Tools → Network Interface menu to change it), ensure that you have **Ethernet** selected. If **Ethernet** is not available in the list, ensure that the radio is on, an Ethernet cable is plugged in, and the Ethernet adapter is working.

**Do not select Local Area Connection, or anything other than Ethernet. They may seem to work, but they are *incorrect***

### Load Firmware NPF Driver/Name Error
This happens when the configuration tool gets confused about which interface to use. The documentation provides this excerpt on it, however I'll go into more detail later:

> If you see an error about NPF name, try disabling all adapters other than the one being used to program the radio. If only one adapter is found, the tool should attempt to use that one. See the steps in Disabling Network Adapters for more info.

As the documentation says, we'll need to disable all network adapters other than the one we're using. To do this, follow these steps:

1. Press Windows + R to open the Run dialog
2. Type in `control`, and press enter
3. Select Network and Internet
4. Select Network and Sharing Center
5. Click `Change adapter settings` on the left panel
6. For each adapter that is not "Ethernet" (or the one you're using, it may be under a different name):
    1. Right-click the adapter
    2. Select `Disable`
7. Ensure that every single adapter other than the one you're using is disabled. It doesn't matter if it seems like it shouldn't affect anything, it will.
8. Close and reopen the Radio Configuration Tool
9. Try to Load Firmware again

### Verification Issues
If you needed to disable your network adapters previously, you may need to re-enable them for verification to work. If during the verification process, an error occurs, try to re-enable your network adapters and try again. If this doesn't work, restart the program and try again -- it may take a couple of tries.

## Helpful Links
- [Official Documentation](https://docs.wpilib.org/en/stable/docs/zero-to-robot/step-3/radio-programming.html)
