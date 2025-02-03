The OSSM is not intended to be a “cheap sex machine” that competes against simple DC motor models on Aliexpress.  Instead, an OSSM is “cheap for what it can do sex machine” that is feature comparable or better than to the most expensive machines on the market with the ability to dynamically set stroke and depth, and move in patterns. 

An OSSM is not a great project to begin your maker journey.  It is more difficult to assemble than IKEA furniture and requires a diverse set of skills that includes 3D printing, mechanical assembly, electronics and possibly programming. 

There are easier and harder ways to build an OSSM.  From easiest to hardest, they are as follows:
- Buy the "ready to play" model from R+D. This is exactly what it says on the box.
- Buy all of the parts from R+D, they've done the sourcing, kitting and 3D printing, all you have to do is put it together.
- Buy some combination of hardware from R+D and stuff you source yourself. 
- Buy only the reference board and remote from R+D, source everything else yourself. 
- (There be dragons beyond this point)
- Have a custom PCB made from the reference design (it's open source!) source all the hardware yourself.
- Design your own special PCB and source all the hardware yourself. (this is much harder than it seems if you're not an EE familiar with building custom boards) 
- Etch the PCB at home, write all your own software... ect. you get the idea

While it is tempting to save money by using unbranded parts, our experience has been that in many cases it is a false economy.  When it is important we will call out specific brands that we know work and are durable.  The more powerful you make your machine the more you need to use quality parts and the stronger things like the stand need to be. 

Find the Bill of Materials (BOM), [here](bom.md)

Use of a reference board is recommended.  Not only it is neater and compatible with community enclosure and mount solutions.  The schematics (eagle files, KiCAD soon!) are available on the github repository or you can purchase it from R&D.  Under the terms of the OSSM MIT license anyone can create and market an OSSM reference board. 

### Motor choice

Check out [this doc](../design/motor.md) for information on motors.

### Motion system

The motion system for the OSSM is based on a 3D printing technology of a GT2 belt drive and linear rail.  This is highly efficient when coupled with a Servo motor compared to the crank based designs and can work well at both high and low speeds. 

Any good quality MGN12**H** rail will work for an OSSM.  While our software supports any length of rail most find that a 350mm version gives a good balance of stroke length (about 170mm) and stability.  Longer rails act like a lever increasing strain on the motor mount to the stand.  This can create the need to reinforce not only the motor clamp but also uprate the stand and adjustment clamps.  Even at 500mm the forces are considerably higher.  Our recommendation is to build with a 350mm first, get the stand working well before scaling up to a longer rail.

Getting a good quality GT2 belt from a company such as Gates is essential for anything but the smallest motors.  Cheap belts have small teeth and wear more quickly than Gates belts and tend to stretch which in turn increases the likelihood of skipping.  

The standard belt width 10mm which is fine for most users.  If you plan on using very large toys a 12mm belt is advantageous.  Just ensure that you increase the size of the pully as well. 

### Power supply

On the KM discord we get more questions about power supplies than any other aspect of the build.  Most people are aware of a rule of thumb that states you need a power supply that exceeds the maximum draw of any component and expect it to apply universally. 

An OSSM is relatively efficient with power consumption and after much real world testing we have arrived at the following specifications:

- 180W JMC Servo or 57AIM30 require a 24V 4 amp PSU

Sourcing a good quality, appropriate power supply is essential.  Like other aspects of the OSSM it important to purchase good quality PSUs from a reputable seller.  Sealed units are preferred for safety as splashes can occur while using an OSSM.  Similarly ensure that all electrical connections are safe and not exposed. 

Our experience has been that Amazon/Aliexpress/eBay are the worst place to purchase PSU
More information about voltage level, power supplies and USB-PD can be found [here](../design/voltage.md)

### Stand

We have an entire section of the docs dedicated to stands, it is quite the topic. See [here](../mounting/index.md)

### End Effector

The effector is the business end of an OSSM and where you mount toys.  There are a number of options that exist both in the official repository and print testing.  Most popular are the various threaded 3D printed options that can be quickly and cheaply printed.  Other choices include click lock that similar to those used by the larger Chinese sex machine companies.   

We have an entire section of the docs dedicated to end effectors. See [here](../end-effectors/index.md)

### Building your OSSM

#### Printing

An OSSM can be printed on most popular 3D Fused Deposition Modelling (FDM) printers if you are not purchasing a kit.  Resin printers typically do not have the necessary layer strength without specialized materials. 

PLA or variation

All models published on the KM github have been tested.  Prior to starting your 3D printing, ensure your printer is well calibrated.


# TODO, the following sections...
Assembly

Testing

Using you OSSM

Designing for OSSM

Getting support