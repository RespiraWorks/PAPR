# RespiraWorks PAPR Project

![Overview photo](PAPR-protoV7.jpg)

This is a low-cost 3D-printable PAPR project by Edwin Chiu (github: inceptionev)

Most of the work is being done in the sandbox folder for now.  Once things are tested and working, files and instructions will move into the releases folder.  Most of the 3D files here were created in FreeCad v0.18.

I am making this for myself, and for my loved ones who are medical workers and essential workers.  They wear masks all day to keep us safe, and supplies of disposable PPE are not keeping up.

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

### (Work-in-Progress) Bill of Materials:
| Item | Quantity | Manufacturer  | Part #              | Price (USD)     |  Sources       | Notes |
| ---- |---------:| ------------- | ------------------- | ------------:|----------------| ----- |
| papr1   | 1 | Custom 3D print | TopLevelPart-Body | $6 (material) | [3D][3d1] | Main Body |
| papr2   | 1 | Custom 3D print | TopLevelPart-BatteryBack | $2 (material) | [3D][3d2]    | Battery Mount |
| papr3   | 1 | Custom 3D print | TopLevelPart-OutletAdapter | $1 (material) | [3D][3d3]    | 22mm Taper Hose Outlet |
| papr4   | 1 | Custom 3D print | TopLevelPart-OutletKey | $6 (material)  | [3D][3d4]    | key to hold the outlet in |
| papr5   | 1 | Custom 3D print | TopLevelPart-MaskAdapter | $2 (material) | [3D][3d5] | Adapter for bayonet-style mask |
| papr6   | 1 | Wonsmart | WS7040-12-X200 | $36 | [A][1ali] | 12V Blower |
| papr7   | 1 | Generic | PotBrushlessController | $10.11 | [A][2ali] | Potentionmeter Brushless Motor Driver |
| papr8   | 1 | Generic | 9V12V USB-C Trigger | $3.15 | [A][3ali] | USB-C 12V/9V PD Trigger |
| papr9   | 1 | Amazon | 6-inch USB-C Cable | $3.50 | [Z][1azmn] | 6-inch USB-C Cable |
| papr10   | 1 | Amazon | Carry Strap | $12.59 | [Z][2amzn] | Carry Strap |
| papr11   | 1 | Vishay | SA9.0CA-E3/54 | $0.42 | [K][1dk] | TVS diode |
| papr11   | 1 | ON Semi | MUR420G | $0.42 | [K][2dk] | Reverse Protection Diode |
| papr12   | 1 | Amazon | Elastic Phone Holder | $10 | [Z][3amzn] | Elastic band to hold battery |
| papr13   | 1 | Conxwan | 26800mAh battery | $27 | [Z][4amzn] | 18W USB-C Battery |
| papr14   | 3 | Amazon | 6-32 x 3/8" Screws | $8.75 | [Z][5amzn] | Screws to secure back |
| papr15   | 1 | Amazon | 4ft CPAP hose | $10.57 | [Z][6amzn] | CPAP hose |
| papr16   | 1 | 3M | 7093 Filter Cartridge (pair) | $30 | [3M][3m1] | example filter packs |
| papr17   | 1 | 3M | 6200 Respirator Mask | $35 | [3M][3m2] | example respirator mask |
| papr18   | about 10x10cm | Lazy Dog | 1/8" Neoprene Material | $15.80/roll | [Z][7amzn] | gasket material |
| papr19   | 1 | OWO | (Optional) Upgraded potentiometer| $1.00 | [A][4ali] | nicer pot with knob and jam nut |

### Tools
| Item | Quantity | Manufacturer  | Part #              | Price (USD)     |  Sources       | Notes |
| ---- |---------:| ------------- | ------------------- | ------------:|----------------| ----- |
| papr-tool1   | 1 | Custom 3D print | InletGasketJigInsideV1 | $1 (material) | [3D][3d5] | Jig for cutting inlet gasket |
| papr-tool2   | 1 | Custom 3D print | InletGasketJigOutsideV1 | $1 (material) | [3D][3d6] | Jig for cutting inlet gasket |

**Other Useful Tools**
- Exacto blade
- 6-32 tap
- Philips screwdriver
- Small flat-blade screwdriver (for removing outlet key)

[3d1]: https://github.com/RespiraWorks/PAPR/blob/master/sandbox/PAPR-MAIN-V7.FCStd
[3d2]: https://github.com/RespiraWorks/PAPR/blob/master/sandbox/PAPR-MAIN-V7.FCStd
[3d3]: https://github.com/RespiraWorks/PAPR/blob/master/sandbox/PAPR-MAIN-V7.FCStd
[3d4]: https://github.com/RespiraWorks/PAPR/blob/master/sandbox/PAPR-MAIN-V7.FCStd
[1ali]: https://www.aliexpress.com/item/32980201709.html
[2ali]: https://www.aliexpress.com/item/4001161829981.html
[3ali]: https://www.aliexpress.com/item/4000528106092.html
[1azmn]: https://www.amazon.com/gp/product/B01LONPUM4
[2amzn]: https://www.amazon.com/gp/product/B06XDNR14N
[1dk]: https://www.digikey.com/product-detail/en/vishay-semiconductor-diodes-division/SA9.0CA-E3-54/SA9.0CA-E3-54GICT-ND/3847567
[2dk]: https://www.digikey.com/product-detail/en/on-semiconductor/MUR420G/MUR420GOS-ND/1482828
[3amzn]: https://www.amazon.com/gp/product/B07QTHFNYF
[4amzn]: https://www.amazon.com/gp/product/B08729Z2JX
[5amzn]: https://www.amazon.com/Stainless-Lengths-Available-Machine-Phillips/dp/B0793D86TB
[3d5]: https://github.com/RespiraWorks/PAPR/blob/master/sandbox/InletGastketJigs.FCStd
[3d6]: https://github.com/RespiraWorks/PAPR/blob/master/sandbox/InletGastketJigs.FCStd
[6amzn]: https://www.amazon.com/gp/product/B01DJGLEUG
[3m1]: https://www.3m.com/3M/en_US/company-us/all-3m-products/~/3M-Particulate-Filter-7093-P100-60-EA-Case/?N=5002385+3294776429&rt=rud
[3m2]: https://www.3m.com/3M/en_US/company-us/all-3m-products/~/3M-Half-Facepiece-Reusable-Respirator-6200-07025-AAD-Medium-24-EA-Case/?N=5002385+3294780295&preselect=3293786499&rt=rud
[7amzn]: https://www.amazon.com/gp/product/B07BKP6KFX
[4ali]: https://www.aliexpress.com/item/10000192070172.html


## Basic Assembly Narrative (needs to be updated with photos and details)

- **Step 1:** Print out all the 3D printed parts and tools.  Tip: Select the print orientation such that supports fall on flat/inside faces, and avoid supports on text.  Note that depending on your printer, you may need to chase the screw threads with a 6-32 tap.

*photo here: suggested print orientations*

The next few steps can be done while the parts are being printed.  The first part you need is the Gasket Jigs so if you print those first you can get moving.  The next part is the body, followed by the outlet adapter, and the outlet adapter key, and finally, the battery back.  The mask adapter can be printed separately, but it fits in nicely with the outlet adapter and outlet adapter key print.

- **Step 2:** Add diodes to the USB-C PD trigger.  These diodes protect the battery from damaging voltage kickback from the motor driver.  The zener diode has a symmetrical arrangement, so it does not have a polarity, either way is fine.  For the general purpose diode, make sure the side with the line goes to positive (+) on the trigger.  You can use the included holes to mount the diodes.  Then solder the motor controller wires to the pads on the trigger.  You may wish to trim these wires to make them pack better.  Heat shrink anound the trigger assembly.

*photo of this process*

- **Step 3:** Cut, solder, and heat shrink the motor driver to the blower.  Make sure to observe the right pin assignments as pictured or the blower will spin backwards.

*photo of the correct arrangement*

*photo of the finished electronics*

- **Step 4:** Use the gasket jigs to cut out a gasket from the neoprene material

*photos here of how it is done*

- **Step 5:** remove the potentiometer from the motor driver and place it into the slot.  Secure it with some hot glue.  (Optional: if you got the upgraded potentiometer, remove the knob and jam nut, insert the potentiometer, then secure it with the jam nut instead of the glue, and then put the knob back onto the shaft.)  Route the wires back to the electronics pocket.

*photos: installing the potentiometer*

- **Step 6:** Put the gasket into the blower pocket and place the blower

*photo here of gasket and blower placement*

- **Step 7:** Insert the Outlet Adapter and secure it using the Outlet Adapter Key.  If for some reason you need to remove the outlet adapter key, wedge a screwdriver into the provided notch and lever it out.

*photos of here of how this works*

- **Step 8:** Route the wires back to the eletronics pocket

*photo showing routing*

- **Step 9:** Connect the USB-C cable and the potentiometer, and tuck in the electronics

*photo showing arrangement*

- **Step 10:** Route the USB cable up to the slot in the enclosure, being careful not to catch the USB conenctor in a place that is narrower than its height.

- **Step 11:** Place the battery back, being careful not to pinch any wires.

- **Step 12:** Use the screws to secure the battery back onto the body

- **Step 13:** Install the battery in to the PAPR and secure it with the elastic cage.

- **Step 14:** Plug in and test!

18 July 2020 Update:

![Front Exploded View](ExplodedViewFront-protoV7.PNG)

![Back Exploded View](ExplodedViewBack-protoV7.PNG)

![This one protects me](PAPR-protoV7-protectsMe.jpg)

![This one protects you](PAPR-protoV7-protectsYou.jpg)

10 July 2020 Udpate:

![Front Exploded View](20200710-Exploded-View-Screenshot-Front.PNG)

![Back Exploded View](20200710-Exploded-View-Screenshot-Back.PNG)

![3DprintParts](3DprintParts.jpg)
