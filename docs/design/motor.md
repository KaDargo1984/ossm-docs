# Why a Servo
Servos and steppers serve similar purposes and operate on similar principles. Both are permanent magnet electric motors but steppers are designed for high-precision, low-speed use cases that require strong holding torque. A stepper motor's initial torque is much higher than a servo but drops off significantly as speed increases. A servo will have a much lower continuous torque but will maintain that torque throughout its speed range. Servos are also necessarily closed loop, meaning they will continue to provide torque when stopped and can react to changes in resistance. An open-loop stepper can lose steps and on a system such as the OSSM, this WILL cause a crash. 

Unlike a DC motor that is efficient only at certain speeds a servo maintains torque throughout the speed range.  Add to the efficiency of the OSSM belt design a far smaller motor is required compared to the more common DC machines. 

The recommendations the project makes are based on “real world testing” over a two year period, not armchair engineering that uses rule of thumb.  Our biggest findings was that the majority of people don’t need the largest JMC servo or a high amperage power supply (more on this later). 


# Motors
## IHSV57-30-x-36
The IHSV57 is a 36V integrated AC servo made by JMC and comes in 3 sizes, related to the maximum rated power: 100W, 140W and 180W. As the price difference between the three sized was minimal and the 180W version left more room between the mounting face and the control box; the IHSV57-30-18-36 was the standard recommended motor until recently. While the motor is rated for 36v there have been multiple reports of the encoder inside the motor failing at voltages greater than 30v. A 24v power supply or 20v USB-C PD supply is more than sufficient. 

## 57AIM30 (Gold Motor)
The 57AIM30 is also a 36V integrated AC servo. It is part of a larger family of AIM motors from the 42AIM10 to the 60AIM40. The 57AIM30 was chosen as a replacement for the IHSV57 for the following reasons: 
- Cheaper (20%) - dependent on availability and location.
- Smaller (40% length of 180W standard - i.e. 60% reduction!).
- No bulky control box
- Lighter (50% weight of 180W).
- Higher peak force (30% higher in real-world test).
- Better over-torque handling - can be configured to reduce torque output instead of disable like IHSV57.
- Is drop-in replacement for iHSV57 series making BOM compatible.
