# Frequently Asked Questions

### Q: What is OSSM?

A: An OSSM is compact sex machine that can be customized to suit you. It is based around a NEMA23 closed loop servo motor that allows for dynamic changes in speed, depth and position.

### Q: How much does an OSSM cost?

A: That depends. R+D sells a fully assembled, ready-to-play version which varies slightly in price based on exchange rates and material costs. If you source all the components yourself, the OSSM usually comes out to between $300 and $400 USD. Add in a mounting solution and it can approach $500. This is far below the cost of any commercially available fucking machine with similar features. 

### Q: Why go to all this trouble?  Why don't you just buy a ready made machine?

A: The OSSM is open source, capable and extensible. The parts can be purchased locally and the number of custom parts is kept to a minimum.  Best of all you can fully control the stroke speed and most importantly depth.  You can make patterns or even your own control software. There is a vibrant and creative community dedicated to building add-ons and using the OSSM in new and interesting ways. 

### Q: What parts do I need?

A: TODO Add the BOM
  
### Q: I've been reading about motors and now I'm really confused
  
A: If you're confused, the recommended 57AIM30 is probably the right choice for you. Check out the [motors](motors/index.md) for detailed information about the motor choices. 
### Q:  I am a size queen and I don't think the IHSV57 or 57AIM30 will be sufficient for my use, what is the upgrade path?

A: You're not alone! There is work being done on larger, more powerful hardware implementations. Check out the discord for more information.
### Q: Hold on, why does anal play need more powerful motors?

A: Butts have big powerful muscles! It's common for people to bear down, or clench when things are feeling really good. Also it can be pretty fun shoving big objects in there! It can take a big motor to handle a big toy in a powerful butt.

### Q: What sized 3D printer do I need?

A: The minimum bed size is 105mm x 105mm for the largest single piece. Approximately 125mm of height is required for the shorter vac-u-lock compatible adapter, the plate is significantly shorter.

### Q: What print material is best?

A: All of our testing has been with simple PLA, however if you do print it in an interesting material make sure to share it to the discord!

### Q: What is the infill percentage?

A: 30% has been found to work just fine with PLA for non flexible parts

### Q: How thick are the walls and top?

A: Recommend at least 3mm for non flexible parts.

### Q: What are these flexible parts and how should I print them?

A: There are mounting solutions that use clamps for the OSSM these need some flexibility.  For these parts thinner walls 2mm, lower infill percentages and a gyroid pattern.

### Q: How do I mount toys onto the OSSM?

A: The standard OSSM implementation uses a 24mm threaded end effector, a vac-u-lock compatible attachment called the double-bubble can be screwed on, or a flat plate that any dildo can be lashed to can be screwed on. Since the 24mm end effector is standardized, you can put anything you can design on it. 

### Q: What to I mount the machine on?  

A: Check out [Mounting](mounting/index.md)
### Q: How do I control my OSSM

A: It depends on how you are going to use it.  Basic OSSM control is via the wired remote and a more advanced remote is available from community members ([M5 Remote](electronics/m5.md)).  The control protocols are open source though, so the sky is the limit if you want to develop your own control system.
### Q: I heard somewhere you can "control via a web page?"  Can I get people to control my OSSM over the internet?

A: As of January 2025 you cannot control an OSSM over the internet.  In the past R&D offered a web page that allowed very basic control with speed and depth settings over wifi. Development is in progress to allow this

### Q: X-Toy and funscript support.  Where is it?  

A: As of January 2025 there is a highly experimental X-toy firmware forked from an earlier version that requires endstops.  This code has significant issue and is not considered to be safe for use on humans. There are frequent pauses, it loses track of where it is and has a tendency to randomly extend to maximum depth. Development of an X-Toys firmware is happening but it is complicated.

### Q: Why is X-Toys/Funscripts/ButtplugIO so difficult?

A: Things are a lot more complicated once you dig down into them.

- The motion core does not yet support position streaming. This is in development and requires a complete redesign of the safety architecture as you don't want to accidentally stab yourself.
- From the experimental software we learnt that the latency margin is really thin, Bluetooth especially struggles here. This will be a challenge to overcome.
- The data models of both xtoys and Buttplug.io do not support complex data models as it would be required for OSSM out of the box. As scaling to the full length of OSSM is just not an option. There might be a workaround by emulating an other toy. But you won't be able to control all aspects of OSSM through this.

### Q: There is an OSSM reference board do I have to buy it to make an OSSM?

A: No you don't but it does make building an OSSM a lot easier and stops you having to solder anything.  

### Q: Power supplies what size do I need?

A: See the following [Document](design/voltage.md)

### Q: How long should the H-rail be?

A: It is really up to you but a 350mm rail will give approximately 195mm of depth.  

### Q: What is the size of the 24mm Thread for the End Effector?

A: It is a M24x3 (this is the size on the machine, do a test print for your new End Effector, you may have to upsize by 3-5%)
