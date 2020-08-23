# RespiraWorks PAPR Project

![Overview photo](/assets/PAPR-protoV7.jpg)

This is a low-cost 3D-printable PAPR project started by Edwin Chiu as part of RespiraWorks (github: inceptionev)

This project is currently at release-candidate stage.  The current files can be found in the release-candidates folder.  Most of the 3D files here were created in FreeCad v0.18.

The most current instructions are those in this README.  They include instructions both for building the PAPR and for modifying off-the-shelf masks, hoods, and helmets for use with the PAPR.

I am making this for myself, and for my loved ones who are medical workers and essential workers.  They wear masks all day to keep us safe, and supplies of disposable PPE are sometimes uncertain.

The combination of a respirator mask, powered air delivery, and commonly-available bayonet-mount filter packs provides a better face-seal, more comfortable breathing, and more re-usability than disposable masks. 

## Features:
- Uses commonly-available 6000-series or 7093 bayonet filter packs, which have many options in N95, P95, and P100 types.
- Powered by a USB-C PD battery pack (as long as it is 9V @ 2.0A capable)
- Packs can be swapped out for 8hrs+ of runtime per 20000mAH battery.
- If used with a modified respirator mask, it can be made to filter both inhaled and exhaled air.
- It can be used with a variety of full-head hoods, full-face masks, and respirator masks.

Also have a look at RespiraWorks' Ventilator project at https://respira.works and https://github.com/RespiraWorks/Ventilator

### Purchasing Source Key

* **A** = Aliexpress
* **C** = McMaster-Carr
* **W** = Wonsmart
* **K** = Digikey
* **3D** = 3D printed
* **Z** = Amazon
* **R** = RS computing
* **3M** = 3M
* **G** = Grainger

### Bill of Materials:
| Item | Quantity | Manufacturer  | Part #              | Price (USD)     |  Sources       | Notes |
| ---- |---------:| ------------- | ------------------- | ------------:|----------------| ----- |
| papr1   | 1 | Custom 3D print | TopLevelPart-Body | $6 (material) | [3D][3d1] | Main Body |
| papr2   | 1 | Custom 3D print | TopLevelPart-BatteryBack | $2 (material) | [3D][3d2]    | Battery Mount |
| papr3   | 1 | Custom 3D print | TopLevelPart-OutletAdapter | $1 (material) | [3D][3d3]    | 22mm Taper Hose Outlet |
| papr4   | 1 | Custom 3D print | TopLevelPart-OutletKey | $6 (material)  | [3D][3d4]    | key to hold the outlet in |
| papr5   | 1 | Custom 3D print | TopLevelPart-MaskAdapter | $2 (material) | [3D][3d5] | Adapter for bayonet-style mask |
| papr6   | 1 | Wonsmart | WS7040-12-X200 | $36 | [A][1ali] | 12V Blower |
| papr7   | 1 | Generic | PotBrushlessController | $10.11 | [A][2ali] | Potentiometer-Controlled Brushless Motor Driver |
| papr8   | 1 | Generic | 9V/12V USB-C Trigger | $3.15 | [A][3ali] | USB-C 12V/9V PD Trigger |
| papr9   | 1 | Amazon | 6-inch USB-C Cable | $3.50 | [Z][1azmn] | 6-inch USB-C Cable |
| papr10   | 1 | Amazon | Carry Strap | $12.59 | [Z][2amzn] | Carry Strap |
| papr11   | 1 | Littelfuse | SMAJ9.0A | $0.41 | [K][1dk] | TVS diode |
| papr11   | 1 | Various | CAP 0805 4.7uF 50V X5R | $0.27 | [K][2dk] | Filtering Cap - manufacturer stock rotates often, so search for an in-stock part |
| papr12   | 1 | Amazon | Elastic Phone Holder | $10 | [Z][3amzn] | Elastic band to hold battery |
| papr13   | 1 | Conxwan | 26800mAh battery | $27 | [Z][4amzn] | 18W USB-C Battery |
| papr14   | 3 | Amazon | 6-32 x 3/8" Screws | $8.75 | [Z][5amzn] | Screws to secure back |
| papr15   | 1 | Amazon | 4ft CPAP hose | $10.57 | [Z][6amzn] | CPAP hose |
| papr16   | 1 | 3M | 7093 Filter Cartridge (pair) | $30 | [3M][3m1] | example filter packs |
| papr18   | about 6x6cm | McMaster-Carr | 8785K82-8785K822 (Extra Soft)  | $22.22/12x12" | [C][1mcmc] | 1/8" Silicone Foam Gasket Material |
| papr19   | 1 | 3M | Inlet Filter Gasket  | $2.01 | [G][1grgr] | Inlet Gasket for 6000-series filters |
| papr20   | 1 | OWO | (Optional) Upgraded potentiometer| $1.00 | [A][4ali] | nicer pot with knob and jam nut |
| papr21   | 1 | JST | (Optional) JST connector kit and crimper | $40 | [Z][8amzn] | required connectors for upgraded potentiometer |


### Mask/Helmet Parts
Parts for modifying and adapting masks and helmets for use with the PAPR

| Item | Quantity | Manufacturer  | Part #              | Price (USD)     |  Sources       | Notes |
| ---- |---------:| ------------- | ------------------- | ------------:|----------------| ----- |
| mask1   | 1 | 3M | 6100(S)/6200(M)/6300(L) Respirator Mask | $35 | [3M][3m2] | example half-face respirator mask* |
| mask2   | 1 | 3M | 6700(S)/6800(M)/6900(L) Full-Face Mask | $150 | [3M][3m3] | example full-face respirator mask* |
| mask3   | 1 | 3M | M-206 Full Face Helmet | $230 | [3M][3m4] | example full-face respiratory helmet* |
| mask4   | 1 | Allegro | Tyvek Full-Face Hood | $23 | [Z][9amzn] | example full-face hood* |
| mask5   | 1 | Custom 3D print | Bayonet Inlet Adapter | $2 (material) | [3D][3d7] | Inlet Adapter for Bayonet-type masks |
| mask6   | 1 | Custom 3D print | 6100/6200/6300 Outlet Plug | $1 (material) | [3D][3d8] | Plug for sealing the outlet valve of 6100/6200/6300 masks |
| mask7   | 1 | 3M | Inlet Filter Gasket  | $2.01 | [G][1grgr] | Inlet Gasket used as part of above outlet sealing |
| mask8   | 1 | Custom 3d print | Male Garden Hose Thread Adapter for Outlet  | $1.01 | [3d][1grgr] | MGHT adapter sealing |

*note, without modification, these masks do not filter the exhaled air.  They are useful for keeping the wearer safe, but not for keeping others safe from the wearer.

Some of these can be modified enable full 2-way filtering.  Instructions are planned for this lower down on this page.


### Tools and useful consumables
| Item | Quantity | Manufacturer  | Part #              | Price (USD)     |  Sources       | Notes |
| ---- |---------:| ------------- | ------------------- | ------------:|----------------| ----- |
| papr-tool1   | 1 | Custom 3D print | InletGasketJigInsideV1 | $1 (material) | [3D][3d5] | Jig for cutting inlet gasket |
| papr-tool2   | 1 | Custom 3D print | InletGasketJigOutsideV1 | $1 (material) | [3D][3d6] | Jig for cutting inlet gasket |

**Other Useful Tools**
- Exacto blade
- 6-32 tap
- Phillips screwdriver
- Small flat-blade screwdriver (for removing outlet key)
- Assorted heat-shrink tubing or electrical tape
- Soldering iron and soldering supplies
- Small, 2mm thick needle file

[3d1]: https://github.com/RespiraWorks/PAPR/blob/master/release-candidates/PAPR-Rev9/PAPR-Body-V9.stl
[3d2]: https://github.com/RespiraWorks/PAPR/blob/master/release-candidates/PAPR-Rev9/PAPR-BatteryBack-V9.stl
[3d3]: https://github.com/RespiraWorks/PAPR/blob/master/release-candidates/PAPR-Rev9/PAPR-OutletAdapter-V9.stl
[3d4]: https://github.com/RespiraWorks/PAPR/blob/master/release-candidates/PAPR-Rev9/PAPR-OutletKey-V9.stl
[1ali]: https://www.aliexpress.com/item/32980201709.html
[2ali]: https://www.aliexpress.com/item/4001161829981.html
[3ali]: https://www.aliexpress.com/item/4000528106092.html
[1azmn]: https://www.amazon.com/gp/product/B01LONPUM4
[2amzn]: https://www.amazon.com/gp/product/B06XDNR14N
[1dk]: https://www.digikey.com/product-detail/en/littelfuse-inc/SMAJ9.0A/SMAJ9.0ALFCT-ND/762476
[2dk]: https://www.digikey.com/product-detail/en/samsung-electro-mechanics/CL21A475KBQNNNE/1276-1248-1-ND/3889334
[3amzn]: https://www.amazon.com/gp/product/B07QTHFNYF
[4amzn]: https://www.amazon.com/gp/product/B08729Z2JX
[5amzn]: https://www.amazon.com/Stainless-Lengths-Available-Machine-Phillips/dp/B0793D86TB
[3d5]: https://github.com/RespiraWorks/PAPR/blob/master/release-candidates/tools/InletGasketJigInsideV1.stl
[3d6]: https://github.com/RespiraWorks/PAPR/blob/master/release-candidates/tools/InletGasketJigOutsideV1.stl
[6amzn]: https://www.amazon.com/gp/product/B01DJGLEUG
[3m1]: https://www.3m.com/3M/en_US/company-us/all-3m-products/~/3M-Particulate-Filter-7093-P100-60-EA-Case/?N=5002385+3294776429&rt=rud
[3m2]: https://www.3m.com/3M/en_US/company-us/all-3m-products/~/All-3M-Products/Personal-Protective-Equipment/Reusable-Respirators/Half-Facepiece-Respirators/3M-Half-Facepiece-Reusable-Respirators-6000-Series/?N=5002385+8711017+8720539+8720550+8720785+8726639+3294857497&rt=r3
[7amzn]: https://www.amazon.com/gp/product/B07BKP6KFX
[4ali]: https://www.aliexpress.com/item/10000192070172.html
[8amzn]: https://www.amazon.com/gp/product/B07R1H3Z8X
[1mcmc]: https://www.mcmaster.com/8785K82-8785K822/
[3m3]: https://www.3m.com/3M/en_US/company-us/all-3m-products/~/All-3M-Products/Personal-Protective-Equipment/Reusable-Respirators/Full-Facepiece-Respirators/3M-Full-Facepiece-Reusable-Respirators-6000-Series/?N=5002385+8711017+8720539+8720550+8720784+8726633+3294857497&rt=r3
[3m4]: https://www.3m.com/3M/en_US/company-us/all-3m-products/~/3M-Versaflo-Respiratory-Faceshield-Assembly-M-206-37299-AAD-with-Comfort-Faceseal-1-EA-Case/?N=5002385+3292194464&preselect=3293786499&rt=rud
[9amzn]: https://www.amazon.com/gp/product/B012D8N4I6/
[1grgr]: https://www.grainger.com/product/3M-Inhalation-Port-Gasket-3PRG7
[3d7]: https://github.com/RespiraWorks/PAPR/blob/master/release-candidates/PAPRmasks/PAPRmasks-BayonetInletAdapter-V1.stl
[3d8]: https://github.com/RespiraWorks/PAPR/blob/master/release-candidates/PAPRmasks/PAPRmasks-6200-OutletPlug-V1.stl

## PAPR Assembly Instructions

**Step 1:** Print out all the 3D printed parts and tools.  Tip: Select the print orientation such that supports fall on flat/inside faces, and avoid supports on text.  Note that depending on your printer, you may need to chase the screw threads with a 6-32 tap.

The PAPR was designed and tested using the following setup.  You may need to make modifications for your printer/material/setup.
- Printer: Elegoo Mars (SLA LCD Masking 3D Printer)
- Material: Blend of 30% Siraya Tech Tenacious and 70% Siraya Tech Fast Grey
 - This blend makes a material that is strong but also slightly flexible and thus resistant to cracking due to impacts.
- Layer Thickness: 0.05mm
- Exposure time (bottom layers): 30s
- Expposure time (all other layers): 8s

**Suggested Print Orientations**

**Body**
- Tilt angle: 3.75° lean back
- This allows the supports to come in at an angle that makes them easier to remove.
- This is the maximum angle that still allows the supports needed to correctly print the bayonet teeth in the inlet.
- This orientation preserves the quality of the printed text.

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Print Orientation: Body Front](/assets/PrintOrientations1-BodyFront.PNG) | ![Print Orientation: Body Back](/assets/PrintOrientations2-BodyBack.PNG) |

**Battery Back**
- Tilt angle: 11° lean back
- These minimal supports were confirmed to print reliably with the settings above.
- This orientation keeps the inside surface of the back flat, which is required for pushing the blower into the gasket.

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Print Orientation: Battery Back Front](/assets/PrintOrientations3-BatteryBackFront.PNG) | ![Print Orientation: Body Back Back](/assets/PrintOrientations4-BatteryBackback.PNG) |

**Small Parts**
- Only the outlet adapter and outlet key are required to build the PAPR, but if you are making the 6100/6200/6300 mask mods, you can combine the inlet adapter and outlet plug on this print.
- Tilt angle: 4° on the mask inlet adapter only.  This overhangs the front face, allowing supports to reach the engagement teeth.
- These supports on the mask inlet adapter are necessary to make those teeth print correctly.
- Supports are necessary on the outlet adapter as well, to prevent vacuum formation, which can distort or fail the print.
- Supports are not technically necessary on th outlet plug and outlet key, but the rafts make removal from the build plate easier, and prevent bottom layer over-exposure distortions which you would otherwise need to remove during post-processing.

![Print Orientation: Small Parts](/assets/PrintOrientations5-SmallParts.PNG)


**Other Printing Tips:**

- Good curing is key.  I recommend 60min under 405nm 6W lights minimum.  Turn your parts to make sure no portions stay shadowed during curing.
- Keep the alcohol wash short, 5min maximum.  Parts left in alcohol for too long will swell and lose strength.  
- The next build steps can be done while the parts are being printed.  
- The first part you will need in the process is the Gasket Jigs so if you print those first you can get moving.  The next part is the body, followed by the outlet adapter and the outlet adapter key, and finally, the battery back. 
- You may need to chase the threads in the body with a 6-32 tap.
- Having a 2mm thick needle file can be useful for clearing residue from the supports in the outlet adapter key slot.

**Step 2:** Gather your electrical parts.

![Electrical Parts](/assets/ElectricalAssembly1-Parts.jpg)

**Step 3:** Prepare the PD Trigger.  Here will we set the voltage to 9V and add voltage protection to the output.  

Removing the solder bridge sets the PD mode to 9V.

The diode and cap are necessary to protect the battery from receiving damaging voltage kickback from the motor driver.  

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Trigger Voltage and Diode](/assets/ElectricalAssembly2-Diode.jpg) | ![Diode Detail](/assets/ElectricalAssembly3-DiodeDetail.jpg) |

The diode has a line indicating the cathode.  Make sure the side with the line goes to positive (+) on the trigger.  

Now flip the PD Trigger over and solder the 4.7uF 50V cap to the backside between the two metal thru-holes.

![Cap](/assets/ElectricalAssembly4-Cap.jpg)

Then solder the motor controller wires to the pads on the trigger.  Heat shrink anound the completed trigger assembly.

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Power Wires](/assets/ElectricalAssembly5-PowerWires.jpg) | ![PD Trigger Heat Shrink](/assets/ElectricalAssembly6-PowerHeatshrink.jpg) |

**Step 4:** Attach the driver to the blower.  Make sure to observe the right pin assignments as pictured or the blower will spin backwards.

Cut the White, Yellow, and Blue blower wires near the connector, preserving as much length as possible.  Cut some heat shrink tubing and put them on the blower wires before you proceed.

Trim the driver's black phase wires short and strip them as pictured.  Solder the blower and driver phase wires as pictured, being mindful of the driver orientation (capacitors below wires).  Apply the heat shrink tubing.

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Phase Wires](/assets/ElectricalAssembly7-PhaseWires.jpg) | ![Phase Wires Heat Shrink](/assets/ElectricalAssembly8-DriverHeatshrink.jpg) |

**Step 5:** Install the pot into the body.  If you are using the included pot that comes with the driver, most of these steps will be optional.  For the included pot, push the pot into the slot and through the shaft hole, and glue it in place with some hot glue.  If you are using the upgraded pot with knob, follow these instructions:

Take the included pot and cut off the wires, preserving the connector and wires.

![Included pot](/assets/ElectricalAssembly9-Pot1.jpg)

Crimp JST XH sockets onto the ends of these pins.  Populate the sockets into a 3-pin female JST XH housing, using the old pot as a guide for the pin arrangement.  Insert the connector into the pot PCB.

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Pot Wire Crimps](/assets/ElectricalAssembly10-Pot2.jpg) | ![Pot Wire Connector](/assets/ElectricalAssembly11-Pot3.jpg) |

Remove the knob, nut, and washer from the pot.  The knob is push-fit and just slides off.  Install it into the slot and through the shaft hole with the PCB up against the inner wall.  Route the wires through the groove.  

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Pot hardware](/assets/ElectricalAssembly12-Pot4.jpg) | ![Pot placement](/assets/ElectricalAssembly13-Pot5.jpg) |

From the other side, install the washer and nut and tighten to retain the pot.  Install the push-fit knob.

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Pot Installation](/assets/ElectricalAssembly14-Pot6.jpg) | ![Knob Installtion](/assets/ElectricalAssembly15-Pot7.jpg) |

Plug the other end of the pot wires into the driver.

![Driver Pot Connection](/assets/ElectricalAssembly16-Pot8.jpg)

**Step 6:** Use the gasket jigs to cut out the inlet gasket from the gasket material.

First, make sure you have enough room to cut out the inlet gasket. Place the inner gasket jig and use it to make the inner cut.

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Gasket Material](/assets/MechanicalAssembly1-Gasket1.jpg) | ![Gasket inner cut](/assets/MechanicalAssembly2-Gasket2.jpg) |

Place the outer gasket jig into the hole you just cut and use it to make the outer cut.

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Outer Gasket Jig](/assets/MechanicalAssembly3-Gasket3.jpg) | ![Gasket outer cut](/assets/MechanicalAssembly4-Gasket4.jpg) |

Insert the completed inlet gasket into the housing.

![Inlet Gasket Placement](/assets/MechanicalAssembly5-Gasket5.jpg)

**Step 7:** Install the blower into the housing.

Put the blower into the pocket over the gasket.

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Place the Blower](/assets/MechanicalAssembly6-PlaceBlower.jpg) | ![Place the Blower](/assets/MechanicalAssembly7-BlowerPlaced.jpg) |

Insert the outlet adapter through the hole at the top of the housing and install the retaining key.

|                            |                             |                             |
|:--------------------------:|:---------------------------:|:---------------------------:|
| ![Outlet Adapter Placement](/assets/MechanicalAssembly8-Outlet1.jpg) | ![Outlet Key Placement](/assets/MechanicalAssembly9-Outlet2.jpg) | ![Outlet Complete](/assets/MechanicalAssembly10-Outlet3.jpg)

Route the wires back through the groove to the electronics pocket.  Fit the driver and PD trigger into this pocket.  Install the 6" USB-C cable into the PD trigger and route it as shown out the top of the housing, being careful not to catch the USB connector in a place that is narrower than its height.

![Electronics Layout](/assets/ElectricalAssembly17-Layout.jpg)

If for some reason you ever need to remove the outlet adapter key, wedge a screwdriver into the provided notch and lever it out.

![Outlet Key Removal](/assets/MechanicalAssembly11-OutletKeyRemoval.jpg)


**Step 8:** Install the battery back, being careful not to pinch any wires.  It's easiest to slide it on, while holding the wires in place. Use the screws to secure the battery back onto the body. Install the battery into the PAPR and secure it with the elastic cage.

|                            |                             |                             |
|:--------------------------:|:---------------------------:|:---------------------------:|
| ![Slide on the Battery Back](/assets/MechanicalAssembly12-BatteryBack1.jpg) | ![Screw on the Battery Back](/assets/MechanicalAssembly13-BatteryBack2.jpg) | ![Battery Install](/assets/MechanicalAssembly14-BatteryBack3.jpg) |


**Step 9:** Take one of the filter gaskets and put it onto the inlet bayonet.

![Inlet Filter Gasket](/assets/MechanicalAssembly15-InletGasket.jpg)

**Step 10:** Install the shoulder strap.

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Install Shoulder straps](/assets/MechanicalAssembly16-ShoulderStrap1.jpg) | ![Install Shoulder Straps](/assets/MechanicalAssembly17-ShoulderStrap2.jpg) |

**Step 11:** Assembly Complete.  Plug in and test!  The blower should spin counter-clockwise.  After confirming proper operation, install the bayonet filter cartridge.  

![Completed Assembly](/assets/Assembly-Complete.jpg)

|                            |                             |
|:--------------------------:|:---------------------------:|
![Install Filter](/assets/MechanicalAssembly18-InstallFilter1.jpg) | ![Install Filter](/assets/MechanicalAssembly19-InstallFilter2.jpg)



## Mask Assembly Instructions

### 6100/6200/6300 Half Facepiece Mask

Note that 6100 is the small side, 6200 is medium, and 6300 is large.  These instructions and the 3D-printed pieces will work with all three sizes.

These modifications to the mask make it compatible with the PAPR, while also plugging the exhale valve and repurposing one of the inlet filters as an outlet filter.  This converts the mask into a full 2-way PAPR that filters both inhaled and exhaled air.

**Step 1:** Select one side of the mask to be the outlet filter side.  Remove the check valve membrane from the one-way valve on that side.  Install the bayonet filter cartridge onto that side.  On the opposite side, leave the valve membrane in place and install the 3D-Printed Bayonet Mask Adapter.

|                            |                             |                             |
|:--------------------------:|:---------------------------:|:---------------------------:|
| ![Remove Valve Membrane](/assets/6200Mask1-RemoveMembrane.jpg) | ![Install Parts](/assets/6200Mask2-InstallParts.jpg) | ![Bayonet Inlet Adapter](/assets/6200Mask3-BayonetInletAdapter.jpg) |

**Step 2:** Remove the outlet valve cover.  A flat bladed screwdriver will help.  Leave the outlet valve membrane in place.  

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Remove Outlet Cover](/assets/6200Mask4-RemoveOutletCover.jpg) | ![Leave Outlet Membrane in Place](/assets/6200Mask5-LeaveMembrane.jpg) |

Put one of the 3M filter gaskets over the membrane, followed by the outlet plug.

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Place Gasket](/assets/6200Mask6-PlaceGasket.jpg) | ![Place Plug](/assets/6200Mask7-PlacePlug.jpg) |

**Step 3:** Reinstall the outlet valve cover, making sure it snaps into place, and mark it as sealed.

|                            |                             |
|:--------------------------:|:---------------------------:|
| ![Reinstall Outlet Cover](/assets/6200Mask8-CloseOutletCover.jpg) | ![Label Outlet](/assets/6200Mask9-LabelOutlet.jpg) |

![Completed Mask](/assets/6200Mask10-MaskComplete.jpg)

### Coming Soon:

Instructions and 3D print files to modify more masks, hoods, and helmets for use with the PAPR.
![Modified Masks](/assets/ModifiedMasks.jpg)

Instructions on how to modify the outlet valves to enable filtering of the exhaled air.
![Outlet Sealed](/assets/Sticker-ClosedOutlet.png)

![Edwin in an M-206 Full Face Helmet](/assets/EdwinInPAPR-M206.jpg)






18 July 2020 Update:

![Front Exploded View](ExplodedViewFront-protoV7.PNG)

![Back Exploded View](ExplodedViewBack-protoV7.PNG)

![This one protects me](PAPR-protoV7-protectsMe.jpg)

![This one protects you](PAPR-protoV7-protectsYou.jpg)

10 July 2020 Udpate:

![Front Exploded View](20200710-Exploded-View-Screenshot-Front.PNG)

![Back Exploded View](20200710-Exploded-View-Screenshot-Back.PNG)

![3DprintParts](3DprintParts.jpg)
