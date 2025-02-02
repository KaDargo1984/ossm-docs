## Bill Of Materials

We are calling this the reference build, when deviating from it please check compatibility with existing Bill Of Materials (BOM)

**[3D Printed Parts](3dprintedparts.md)**
Reference the above for information on choosing, printing and purchasing 3d printed parts

1. **IHSV57 NEMA23 Servo with 8mm shaft** _or_ **57AIM30 (Gold Motor)**:
    - **Gold Motor**
      - New standard motor for OSSM, please see [Gold Motor Info](../motors/57AIM30.md)
      - For the latest information about this change, join the KinkyMakers Discord.
    - **iHSV57 (Previous Standard Motor)**
      - _Avoid the StepperOnline version_
      - Make sure you get something with **8mm** shaft.
      - There are **3** sizes of this motor:  
          100W = [iHSV57-30-**10**](https://www.aliexpress.com/w/wholesale-iHSV57%2525252d30%2525252d10.html)

          140W = [iHSV57-30-**14**](https://www.aliexpress.com/w/wholesale-iHSV57%2525252d30%2525252d14.html)

          180W = [iHSV57-30-**18**](https://www.aliexpress.com/w/wholesale-iHSV57%2525252d30%2525252d18.html)
      - With the move to the 57AIM30, mainline support for the rs232 modbus on the IHSV will not exist. If you want to use the modbus, please ensure you get firmware version 6 or later (shown as `V60x`). The firmware version is printed on the label on the side of the motors control box. You cannot update the motor firmware. 

2.  **GT2 Pulley 8mm Bore 20 Tooth, 10mm width** :

    [Amazon - CA](https://www.amazon.ca/Timing-Pulley-8mm-bore-10mm-belt-20-Tooth/dp/B09L7D7HHT)

    [Amazon - US](https://www.amazon.com/WINSINN-Aluminum-Synchronous-Timing-Printer/dp/B07BTDRW5Z)

    [Banggood - AU](https://au.banggood.com/5MM-or-6_35MM-or-8MM-Bore-20TeethGT2-Alumium-Timing-Pulley-For-Width-10mm-GT2-Belt-p-1106314.html)

3. **GT2 Timing Belt - 10mm width** :

    [Amazon - CA](https://www.amazon.ca/Timing-Meters-Creality-Anycubic-Printer/dp/B097T4DFM6)

    [Amazon - US](https://www.amazon.com/Timing-Meters-Creality-Anycubic-Printer/dp/B097T4DFM6)

    [Amazon - AU]()

    - Your desired stroke length plus about 200mm should be your minimum order length


4. **Bearings** MR115-2RS 5x11x4mm :
    [Amazon - CA](https://www.amazon.ca/gp/product/B07CVBW44R)

    [Amazon - US](https://www.amazon.com/Miniature-Bearings-MR115-2RS-Double-Shielded-5x11x4mm/dp/B08PFT72RQ)

    [Aliexpress - AU](https://www.aliexpress.us/item/2251832628223170.html)

5. **MGN12H Rail and bearing** :

    [Amazon - CA](https://www.amazon.ca/MGN12H-Stainless-Carriage-Precision-Machine/dp/B09TWKWCZR)

    [Amazon - US](https://www.amazon.com/ReliaBot-Linear-Carriage-Printer-Machine/dp/B07B4DWWZC)

    [Aliexpress - AU](https://www.aliexpress.com/item/32840113910.html)

    - Minimum 250mm in length, suggested 350mm
    - Rail length = desired stroke + 180mm
    - Must be MGN**12H** rail - H is a longer carrige than C which gives greater stability. 12 indicates 12mm rail width.

6. **Power Supply**: 24 volt 4-5 amp w/ 2.1mm barrel DC plug OR 20V USB-PD adapter with 2.1mm barrel jack

    - Larger motors generally need more power!  
      180W -> 24V 5A suggested minimum  (also good motor)
      140W -> 24V 4A suggested minimum  
      100W -> 24V 4A suggested minimum

    - See the FAQ for more details about power supply sizing based on real world experience of OSSM users.
    - The OSSM will work with small power supplies, but will be limited on maximum force.
    - Ensure the power supply is fully enclosed and shielded to avoid cross talk from electromagnetic interference (like a laptop power supply).
    - Ensure the power supply has the correct approvals for your location - This really helps ensure performance as well! (UL, CE, etc.)
    - It is strongly recommended that you purchase a good quality PSU such as a Meanwell.

7. **Metric Hex Cap Screws** :  
    [Amazon - CA & US](https://www.amazon.ca/Comdox-500pcs-Socket-Screws-Assortment/dp/B06XQLTLHP)

    [Amazon - AU](https://www.amazon.com.au/VIGRUE-Stainless-Hexagon-Washers-Assortment/dp/B08CK9Y971) (this is a little
    expensive, we are looking for a cheaper alternative)

    - A kit like the ones above will provide what's needed:
    - 4x m5x20
    - 1x m5x12 (can also use m5x20)
    - 10x m3x8
    - 2x m3x16
    - 8x m5 nuts
    - 8x m3 nuts

8. **OSSM Control board**
    - The best choice is [an official OSSM reference PCB](https://research-and-desire.myshopify.com/collections/all/products/ossm-reference-board)
    - If you don't want to use a reference board, see [this](../electronics/custom-board.md)

### Octopart Links for ease of ordering and tracking

A list of non-3d printed supplies in one place. Most of the parts aren't available through the preferred Octopart vendors but it still makes for a convenient list.

[Octopart - Collected Bill of Materials for US Suppliers](https://octopart.com/bom-tool/nfUsbySS)
