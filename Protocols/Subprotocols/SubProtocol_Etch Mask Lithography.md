# Sub-Protocol: Etch Mask Lithography

Description: This document details the protocol for the photolithography used to produce the etch mask used to define the pattern in (deep) reactive ion etching steps in the PIE Foundry MEA microfabrication process. This protocol is tailored for use on Parylene C coated silicon wafers.

## Materials:

* *AZ 12XT-20PL-15 Photoresist*
* *726 MIF Developer*
* *5 mL Polypropylene Syringe (per wafer)*

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

## Parameters

Spinner Recipe Program T  
1st Spin Speed: 500 RPM  
1st Spin Time: 10 seconds

1st Spin Acceleration: acceleration level 8 (1088 RPM)  
2nd Spin Speed: 2000 RPM  
2nd Spin Time: 45 seconds

2nd Spin Acceleration: acceleration level 8 (1088 RPM)

### Soft-Bake:<br>
Temperature: 110 °C<br>Time: 180 seconds 

### Exposure<br>
Dose: 185 mJ/cm<sup>2</sup><br>
Time: 14.8 seconds<br>
Intensity: 12.5 mW/cm<sup>2</sup>

### Post-Exposure Bake

Temperature: 90 °C<br>
Time: 60 seconds

### Develop

Concentration: 726 MIF developer as bottled<br>
Time: 75 seconds (approximate)

## Process:

1. Descum
    1. Descum (clean/roughen) wafers in the asher using the following recipe  :
    2. 125 mT, 100 W, 30 sccm O<sub>2</sub>, 300 seconds
2. Prepare Developer and Water Baths<br>_Note: perform in chemical fume hood_
    1. Prepare a shallow HDPE tray full of DI water, and another with 726 MIF developer
    1. ~250 mL of 726 MIF developer should be sufficient for 6 wafers

3. Dry-Bake<br>_Note: this step should be performed immediately before photoresist deposition_
    1. Bake wafers at 60 °C in an oven under light vacuum (35-40 cmHg) and N¬2 flow (15-20 sccm) for >15 minutes

4. Spin Photoresist<br>_Note: Before coating wafers run 3 “dummy spins” using spare wafers to ensure spinner chamber environment is saturated with solvent from photoresist. This will prevent differences in resist thickness between first and last wafers in a run._
    1. Line sidewalls of spinner with aluminum foil to reduce mess
    2. Center wafer on spinner vacuum chuck using spinner centering tool and engage chuck vacuum
    3. Spinner requires supply of clean dry air for vacuum to engage
    4. Deposit 3 mL of AZ 12XT-20PL-15 photoresist from preprepared syringe onto center of wafer
    5. Ensure there are no air bubbles in resist
    6. Close lid and run program
    7. Spin on 500 RPM for 10 seconds
    8. Spin 2000 RPM for 45 seconds

5. Soft-Bake
    1. Bake the wafer on hotplate for 3 minutes at 110 °C. Calibrate temperature to IR gun and do not rely on hotplate reading
    2. Wafer should be placed in the center of the hot plate with flat facing forward. Use heat shield around hot plate
    3. After baking, store the wafer in black wafer storage box for at least 3 minutes

6. Align, Contact, and Exposure
    1. Set the UV lamp to desired intensity and duration. Targeted dose is 185 mJ/cm<sup>2</sup>. Typical intensity is 12.5 mW/cm<sup>2</sup> (measured at i-line 365 nm) for 14.8 seconds but can be adjusted depending on current lamp intensity
    2. Clean mask aligner vacuum chuck and mask holder of any particles. Remove vacuum O-ring around vacuum chuck if present
    3. Place photomask feature (chrome) side down (facing vacuum chuck). Secure with mask holder vacuum and screw clamps
    4. Place wafer face up and centered on vacuum chuck. Turn on substrate vacuum
    5. Blow mask surface and wafer surface clean of particles with N<sub>2</sub> gun
    6. Engage N<sub>2</sub> purge
    7. Lower mask holder
    8. Raise wafer using Z-axis knob until mask is flush with mask. Engage ball lock
    9. Reduce Z-axis control sensitivity. While looking through aligner microscope on lowest magnification, lower wafer until it just barely disengages with mask. Confirm that wafer is now able to move freely using fine X/Y/θ controls
    10. Moving back and forth between left and right alignment marks, align the angle (theta) of the mask and wafer
    11. Once wafer and mask are aligned in theta, ensure X and Y coordinates are aligned
    12. Increase magnification to higher objective lens then repeat 5.10-5.12
    13. Once satisfied, raise the wafer to contact, confirm alignment has not drifted. Disengage N<sub>2</sub> purge
    14. Expose the wafer by carefully sliding the aligner assembly under the UV lamp. Wait for exposure, then carefully slide the assembly back to starting position
    15. Re-engage N<sub>2</sub> purge. Gently lower the wafer. If the wafer does not move freely, pause, and wait before trying again
    16. Once the wafer moves freely, return Z-axis sensitivity to starting level and lower the wafer completely clear of the mask. Raise the mask holder. Dis-engage substrate vacuum and N<sub>2</sub> purge. Remove wafer

7. Post-Exposure-Bake
    1. Bake the wafer on hotplate for 1 minute at 90 °C. Calibrate temperature to IR gun and do not rely on hotplate reading
    2. Wafer should be placed in the center of the hot plate with flat facing forward. Use heat shield around hot plate

8. Quench in Deionized Water
    1. Immediately place wafer in shallow bath of DI water and let soak for 3 minutes to avoid heating and reduce gas bubble formation

9. Develop
    1. Develop wafer in shallow bath of 726 MIF developer for approximately 75 seconds
    2. Development time is dependent on area of exposed features and will vary between mask-sets
    3. Immediately rinse in DI water bath and rinse 3× in water
    4. Blow dry with N<sub>2</sub>

10. Inspect
    1. Inspect under compound microscope with yellow light filter
