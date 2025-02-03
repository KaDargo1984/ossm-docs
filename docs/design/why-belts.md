The OSSM uses a GT2 style belt system to deliver power from the motor to the linear rail that moves the end effector back and forth. 

# Why use a belt?
### Noise
The belt system is quiet, motor noise and the linear rail are both significantly louder than the noise from the belt moving across the bearings and motor. 
### Cost
1m of genuine Gates GT2 10mm wide belt can be purchased for under $20usd. This is enough to belt to construct 2 standard sized OSSMs. A two pack of 20T GT2 pulleys can be had for less than $15usd. This makes the system extremely cost effective at around $22 for a single OSSM. 
### Availability and Convenience
Due to the widespread proliferation of consumer 3D printers, GT2 belts and pulleys have become commodity items, manufactured by various venders and readily available to the hobbyist. The belts can be cut to any length to support an OSSM of basically any length. Additionally, the belt does not require lubrication. 
### Misalignment
The belt and pulley system can tolerate slight misalignment in any axis with little adverse effects. This might come from the 3D printed parts or a misassembled machine.
### Safety
With the cover on, it is very difficult for anything to be pulled into the belt and pulley. Hair is the most significant safety issue. For more information on safety, see [the safety doc](../safety.md). 
### Strength
A properly tensioned GT2 belt on the OSSM will cause a 180w IHSV57 or a 57AIM30 to stall before jumping teeth. These are the standard motors for an OSSM.

# Why not use a rack and pinion?
### Noise
Rack and pinion systems with straight cut, dry gears are loud. One of the main design goals of the OSSM is to be quiet and unobtrusive. 
### Cost
The long rack required for an OSSM are costly and are only available in fixed lengths. One of the main goals of the OSSM was not to require cutting steel components. 
## Availability and Convenience
Rack and pinion systems are not as widely available as the belt drive system used by the OSSM. They also require lubrication which can get messy.
### Misalignment
Rack and pinons can not tolerate any misalignment other than across their movement axis.
### Safety
Rack and pinions have much more exposed pinch points and are much more likely to pull in hair, clothing or anything else that might dangle nearby.
### Strength
Rack and pinon systems are undoubtedly stronger than belts but this extra strength does not gain anything with the default motors.