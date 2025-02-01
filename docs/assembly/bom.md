## Bill Of Materials

We are calling this the reference build, when deviating from it please check compatability with existing Bill Of Materials (BOM)

1.  **[3D Printed Parts](Hardware/OSSM%20Printed%20Parts)**
    - This has recently had significant changes
    - [Make sure to choose one of the options for the toy adapters](Hardware/OSSM%20Printed%20Parts/end%20effector%20options)
    - There are several mounting options available, the most popular being  
      the [Ulanzi Ball head mount](Hardware/OSSM%20Mounting) or  
      the [Shicks mount](Hardware/OSSM%20Mounting/Shicks%204040%20mount)
    - Thank you @Elims for the [belt tensioner design]( https://github.com/theelims )

2.  **IHSV57 NEMA23 Servo with 8mm shaft** _or_ **57AIM30 (Gold Motor)**:
    - **Gold Motor**
      - New standard motor for OSSM, please see [Gold Motor Info](Documentation/Gold-Motor.md) while docs are being updated.
        This motor is cheaper, more compact and has improved features which are being implemented in OSSM firmware.
      - For the latest information about this change, join the KinkyMakers Discord.
    - **iHSV57 (Previous Standard Motor)**
      - _Avoid the StepperOnline version_
      - Make sure you get something with **8mm** shaft.
      - There are **3** sizes of this motor:  
          100W = [iHSV57-30-**10**](https://www.aliexpress.com/w/wholesale-iHSV57%2525252d30%2525252d10.html)

          140W = [iHSV57-30-**14**](https://www.aliexpress.com/w/wholesale-iHSV57%2525252d30%2525252d14.html)

          180W = [iHSV57-30-**18**](https://www.aliexpress.com/w/wholesale-iHSV57%2525252d30%2525252d18.html)

      - We recommend motors with firmware version 6 (shown as `V60x`). Pay attention to
        this, [the firmware version is printed on the label on the side.](https://user-images.githubusercontent.com/131713378/234460307-1c29c18b-3bb5-4ac9-b66f-0dea9df0acac.png)
        You cannot update the motor firmware. version 5 will work, but it is not as feature rich for potential new
        features.
      - Search around for the best deal for you - we reccommend searching "ihsv57" on Aliexpress.com and choosing the -10
        -14 or -18. Some example listings:

        [AliExpress - US](https://www.aliexpress.us/item/2251832528412325.html)

        [AliExpress - CA & AU](https://www.aliexpress.us/item/32714727077.html)


      - For details on picking the right motor for your use case - check
          this [FAQ](FAQ.md#q--what-strength-of--motor-do-i-need)
      - If you are using the 140W or 180W version it is recommended to use a 10mm wide belt and pulley (see the next two items)


3.  **GT2 Pulley 8mm Bore 20 Tooth, 10mm width** :

    [Amazon - CA](https://www.amazon.ca/Timing-Pulley-8mm-bore-10mm-belt-20-Tooth/dp/B09L7D7HHT)

    [Amazon - US](https://www.amazon.com/WINSINN-Aluminum-Synchronous-Timing-Printer/dp/B07BTDRW5Z)

    [Banggood - AU](https://au.banggood.com/5MM-or-6_35MM-or-8MM-Bore-20TeethGT2-Alumium-Timing-Pulley-For-Width-10mm-GT2-Belt-p-1106314.html)

4.  **GT2 Timing Belt - 10mm width** :

    [Amazon - CA](www.amazon.ca/Timing-Meters-Creality-Anycubic-Printer/dp/B097T4DFM6)

    [Amazon - US](https://www.amazon.com/Timing-Meters-Creality-Anycubic-Printer/dp/B097T4DFM6)

    [Amazon - AU]()

    - Your desired stroke length plus about 200mm should be your minimum order length


5.  **Bearings** MR115-2RS 5x11x4mm :
    [Amazon - CA](https://www.amazon.ca/gp/product/B07CVBW44R)

    [Amazon - US](https://www.amazon.com/Miniature-Bearings-MR115-2RS-Double-Shielded-5x11x4mm/dp/B08PFT72RQ)

    [Aliexpress - AU](https://www.aliexpress.us/item/2251832628223170.html)

6.  **MGN12H Rail and bearing** :

    [Amazon - CA](https://www.amazon.ca/MGN12H-Stainless-Carriage-Precision-Machine/dp/B09TWKWCZR)

    [Amazon - US](https://www.amazon.com/ReliaBot-Linear-Carriage-Printer-Machine/dp/B07B4DWWZC)

    [Aliexpress - AU](https://www.aliexpress.com/item/32840113910.html)

    - Minimum 250mm in length, suggested 350mm
    - Rail length = desired stroke + 180mm
    - Must be MGN**12H** rail - H is a longer car than C which gives greater stability. 12 indicates 12mm rail width.

7.  **Power Supply**: 24 volt 4-5 amp w/ 2.1mm barrel DC plug

    - Larger motors generally need more power!  
      180W -> 24V 5A suggested minimum  
      140W -> 24V 4A suggested minimum  
      100W -> 24V 4A suggested minimum

    - See the FAQ for more details about power supply sizing based on real world experience of OSSM users.
    - The OSSM will work with small power supplies, but will be limited on maximum force.
    - Ensure the power supply is fully enclosed and shielded to avoid cross talk from electromagnetic interference (like a laptop power supply).
    - Ensure the power supply has the correct approvals for your location - This really helps ensure performance as well! (UL, CE, etc.)
    - It is strongly recommended that you purchase a good quality PSU such as a Meanwell.

8.  **Metric Hex Cap Screws** :  
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

9.  **ESP32 Development Board**
    - [An official OSSM reference PCB](https://research-and-desire.myshopify.com/collections/all/products/ossm-reference-board)
    - We do not currently have a best suggestion if you are not using a reference board, most generic development boards are the same
    - We have found that the 3.3v boards may miss steps at high speed, so please use a level shifter as well.
    - To start working on the project, something like this [Adafruit board](https://www.adafruit.com/product/3405) is an excellent place to start.
    - Accessories required for prototyping
      include [Breadboard](https://www.amazon.ca/Breadboard-Solderless-Prototype-Distribution-Connecting/dp/B01EV6LJ7G/ref=sr_1_5?dchild=1&keywords=breadboard&qid=1627823170&sr=8-5)
      and [Dupont Jumpers](https://www.amazon.ca/120pcs-Multicolored-Breadboard-Arduino-raspberry/dp/B01LZF1ZSZ/ref=sr_1_5?dchild=1&keywords=dupont+jumper&qid=1627823220&sr=8-5)

### Octopart Links for ease of ordering and tracking

A list of non-3d printed supplies in one place. Most of the parts aren't available through the preferred Octopart vendors but it still makes for a convenient list.

[Octopart - Collected Bill of Materials for US Suppliers](https://octopart.com/bom-tool/nfUsbySS)
