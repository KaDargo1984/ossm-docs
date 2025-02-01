# Motors
## [IHSV57-30-x-36](ihsv57.md)
The IHSV57 is a 36V integrated AC servo made by JMC and comes in 3 sizes, related to the maximum rated power: 100W, 140W and 180W. As the price difference between the three sized was minimal and the 180W version left more room between the mounting face and the control box; the IHSV57-30-18-36 was the standard recommended motor until recently. While the motor is rated for 36v there have been multiple reports of the encoder inside the motor failing at voltages greater than 30v. A 24v power supply or 20v USB-C PD supply is more than sufficient. 

## [57AIM30 (Gold Motor)](57AIM30.md)
The 57AIM30 is also a 36V integrated AC servo. It is part of a larger family of AIM motors from the 42AIM10 to the 60AIM40. The 57AIM30 was chosen as a replacement for the IHSV57 for the following reasons: 
- Cheaper (20%) - dependent on availability and location.
- Smaller (40% length of 180W standard - i.e. 60% reduction!).
- No bulky control box
- Lighter (50% weight of 180W).
- Higher peak force (30% higher in real-world test).
- Better over-torque handling - can be configured to reduce torque output instead of disable like IHSV57.
- Is drop-in replacement for iHSV57 series making BOM compatible.