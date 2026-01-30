# Sub-Protocol: High Resolution Image Reversal Lithography

Description: This document details the protocol for the high-resolution image reversal lithography used to produce the lift-off profile for metal patterning in the PIE Foundry standard microfabrication process. It is tailored for use on Parylene C coated silicon wafers.

## Materials:

* *AZ5214-E Photoresist*
* *AZ340 Developer*
* *5 mL Polypropylene Syringe (per wafer)*
* *22-Gauge Luer Stub (per wafer)*

## Equipment:

* *OAI Model 200 Contact Mask Aligner and UV Source*
* *Electronic Micro Systems 1000-1 Hot plate*
* *YES CV200RFS Plasma Asher*
* *Laurell Technologies Photoresist Spinner Model WS-400B-6NPP Lite*
* *Vacuum oven with N<sub>2</sub>*
* *UV intensity meter*
* *IR temperature sensor*
* *Wafer centering tool*
* *HDPE trays for developer and water baths*
* *Wafer dipper/holding tool*

## Parameters:

### Spinner Recipe Program P  
1st Spin Speed: 500 RPM  
1st Spin Time: 10 seconds<br>
1st Spin Acceleration: acceleration level 8 (1088 RPM)  
<br>
2nd Spin Speed: 4200 RPM  
2nd Spin Time: 40 seconds<br>
2nd Spin Acceleration: acceleration level 8 (1088 RPM)

### Soft-Bake
Temperature: 110 °C
Time: 60 seconds

### 1st Exposure
Dose: 42 mJ/cm<sup>2</sup>
Time: 3.4 seconds
Intensity: 12.5 mW/cm<sup>2</sup>

### Image-Reversal Bake
Temperature: 110 °C
Time: 63 seconds

### 2nd Exposure
Dose: 280 mJ/cm<sup>2</sup><br>
Time: 22.4 seconds<br>
Intensity: 12.5 mW/cm<sup>2</sup>

### Develop
Concentration: 1:4 AZ340 developer to deionized water (200 mL total volume)<br>
Time: 18 seconds

## Process:

1.  Descum
    1. Descum (clean/roughen) wafers in the asher using the following recipe<br>
   300 mT, 100 W, 115 sccm O<sub>2</sub>, 300 seconds

2. Prepare Developer and Water Baths<br>
_Note: perform in chemical fume hood_
    1. Prepare a shallow HDPE tray full of DI water, and with a 1:4 mixture of AZ340 developer and DI water (200 mL total volume)
    <br> a. 200 mL of developer solution should be sufficient for 2 wafers

3. Dry-Bake<br>
_Note: this step should be performed immediately before photoresist deposition_
    1. Bake wafers at 60 °C in an oven under light vacuum (35-40 cmHg) and N<sub>2</sub> flow (15-20 sccm) for >15 minutes

4. Spin Photoresist<br>
_Note: Before coating wafers run 3 “dummy spins” using spare wafers to ensure spinner chamber environment is saturated with solvent from photoresist. This will prevent differences in resist thickness between first and last wafers in a run._
    1. Line sidewalls of spinner with aluminum foil to reduce mess
    2. Center wafer on spinner vacuum chuck using spinner centering tool and engage chuck vacuum
    <br> a. Spinner requires supply of clean dry air for vacuum to engage
    3. Deposit 3 mL of AZ5214-E photoresist from preprepared syringe onto center of wafer through 22-gauge Luer stub
    <br> a. Ensure there are no air bubbles in resist
    4. Close lid and run program
    <br> a. Spin on 500 RPM for 10 seconds
    <br> b. Spin 4200 RPM for 40 seconds

5. Soft-Bake
    1.Bake the wafer on hotplate for 1 minute at 110 °C. Calibrate temperature to IR gun and do not rely on hotplate reading
    2. Wafer should be placed in the center of the hot plate with flat facing forward. Use heat shield around hot plate
    3. After baking, store the wafer in black wafer storage box for at least 3 minutes

6. Vacuum Contact and Exposure
    1. Set the UV lamp to desired intensity and duration. Targeted dose is 42 mJ/cm<sup>2</sup>. Typical intensity is 12.5 mW/cm<sup>2</sup> for 3.4 seconds but can be adjusted depending on current lamp intensity
    2. Clean mask aligner vacuum chuck and mask holder of any particles. Place vacuum O-ring around vacuum chuck
    3. Place photomask feature (chrome) side down (facing vacuum chuck). Secure with mask holder vacuum and screw clamps
    4. Place wafer face up and centered on vacuum chuck. Turn on substrate vacuum
    5. Blow mask surface and wafer surface clean of particles with N<sub>2</sub> gun
    6. Engage N<sub>2</sub> purge
    7. Lower mask holder
    8. Raise wafer using Z-axis knob until mask appears flush with mask. Lower mask slightly and then use fine x/y/θ controls to center wafer under mask. Re-raise wafer
    9. Turn off substrate vacuum and engage contact vacuum. Open contact vacuum knob until vacuum gauge reads ~5” Hg. You may need to lower N<sub>2</sub> purge to create good seal. Please note, sufficient vacuum is only needed to create good contact between mask and wafer as indicated by appearance of Newton ring diffraction. Use the lowest possible vacuum setting that will achieve this effect
    10. Expose the wafer by carefully sliding the aligner assembly under the UV lamp. Wait for exposure, then carefully slide the assembly back to starting position
    11. Lower the contact vacuum level by turning the knob clockwise. Once closed, turn off the contact vacuum. If the N<sub>2</sub> purge level was decreased, return it to starting level. Re-engage the substrate vacuum and then gently lower the wafer. If the wafer does not move freely, pause, and wait before trying again
    12. Lower the wafer completely clear of the mask. Raise the mask holder. Dis-engage substrate vacuum and N<sub>2</sub> purge. Remove wafer

7. Image-Reversal-Bake
    1. Bake the wafer on hotplate for 63 seconds at 110 °C ± 0.5 °C. Calibrate temperature to IR gun and do not rely on hotplate reading
    <br> a. This step is critical. Avoid any variation in time or temperature
    2. Wafer should be placed in the center of the hot plate with flat facing forward. Use heat shield around hot plate
    3. After baking, store the wafer in black wafer storage box for at least 3 minutes

8. Flood Exposure
    1. Set the UV lamp to desired intensity and duration. Targeted dose is 280 mJ/cm<sup>2</sup>. Typical intensity is 12.5 mW/cm<sup>2</sup> for 22.4 seconds but can be adjusted depending on current lamp intensity
    2. Remove mask from mask holder and store
    3. Place wafer face up and centered on vacuum chuck. Turn on substrate vacuum
    4. Blow wafer surface clean of particles with N<sub>2</sub> gun
    5. Expose the wafer by carefully sliding the aligner assembly under the UV lamp. Wait for exposure, then carefully slide the assembly back to starting position
    6. Dis-engage substrate vacuum. Remove wafer

9. Quench in Deionized Water
    1. Immediately place wafer in shallow bath of DI water and let soak for 3 minutes to avoid heating and reduce gas bubble formation

10. Develop
    1. Develop wafer in 1:4 solution of AZ340 to DI water for 18 seconds with mild agitation
    2. Immediately rinse in DI water bath and rinse 3× in water
    3. Blow dry with N<sub>2</sub>

11. Inspect
    1. Inspect under compound microscope with yellow light filter
