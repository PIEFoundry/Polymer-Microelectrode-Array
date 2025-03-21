# Protocol: Microfabrication of Parylene Microelectrode Arrays

Description: This document details the microfabrication protocol for Parylene microelectrode arrays (MEAs) for the standard multi-project wafer model of the Polymer Implantable Electrode (PIE) Foundry.

_Note: Standard equipment and materials (e.g. tweezers, microscopes, DI water, cleanroom wipes, N<sub>2</sub> gun, scale, etc.) are not listed in materials lists._

Table of Contents

1. [Base Parylene C](#1-base-parylene-c)
   * [Dry-Bake](#11-dry-bake)
   * [Deposit Parylene C](#12-deposit-parylene-c)
   * [Measure Parylene Thickness](#13-measure-parylene-thickness)
   * [Thermal Anneal](#14-thermal-anneal)
2. [Electrode (Metal) Layer](#2-electrode-metal-layer)
   * [Photomask Cleaning](#21-photomask-cleaning)
   * [High Resolution Image Reversal Lithography](#22-high-resolution-image-reversal-lithography)
   * [Descum Wafer](#23-descum-wafer)
   * [Deposit Metal](#24-deposit-metal)
   * [Pattern Metal via Lift-Off](#25-pattern-metal-via-lift-off)
   * [Dry-Bake](#26-dry-bake)
3. [Insulation Parylene C](#3-insulation-parylene-c)
   * [Descum Wafer](#31-descum-wafer)
   * [Silanization](#32-silanization)
   * [Dry-Bake](#33-dry-bake)
   * [Deposit Parylene C](#34-deposit-parylene-c)
   * [Measure Parylene Thickness](#35-measure-parylene-thickness)
4. [Pattern Parylene (Etch #1)](#4-pattern-parylene-etch-1)
   * [Photomask Cleaning](#41-photomask-cleaning)
   * [Pattern Etch Mask with Photolithography](#42-pattern-etch-mask-with-photolithography)
   * [Etch Parylene](#43-etch-parylene)
   * [Strip Photoresist Mask](#44-strip-photoresist-mask)
5. [Pattern Parylene (Etch #2)](#45-dry-bake)
   * [Photomask Cleaning](#5-pattern-parylene-etch-2)
   * [Pattern Etch Mask with Photolithography](#51-photomask-cleaning)
   * [Etch Parylene](#53-etch-parylene)
   * [Strip Photoresist Mask](#54-strip-photoresist-mask)
6. [Release MEAs](#6-release-meas)
7. [Post-Process Annealing](#7-post-process-annealing)
   * [Release Stress (Flatten)](#71-release-stress-flatten)
   * [Vacuum Anneal](#72-vacuum-anneal)
   * [High Temperature Vacuum Anneal](#73-high-temperature-vacuum-anneal)
8. [Post-Process Cleaning](#8-post-process-cleaning)

<ol type="A">
  <li>    <a href="#a-process-flow-diagram">Process Flow Diagram</a>   </li>
  <li>     <a href="#b-material-sources">Material Source</a>   </li>
  <li>     <a href="#c-equipment-models">Equipment Models</a>   </li>
</ol>

## 1. Base Parylene C

### 1.1 Dry-Bake

_Note: this step assumes you are working with new wafers directly taken from the box in which they were shipped in – the assumption is that these wafers are completely clean_

_Note: this step should be performed immediately before Parylene deposition_

Materials:
* *4” prime double-sided-polished 525 micron thick silicon wafer(s) (laser serial marked preferred)*

Equipment:
* *Oven or hotplate*

Process:
1. Bake wafers at 110 °C in an oven at atmosphere for at least 30 minutes (overnight is OK), or on a hot plate for >5 minutes

### 1.2 Deposit Parylene C

_Note: this step should be performed immediately after dry-bake (step 1.1)_

Materials:
* *Parylene C Dimer*

Equipment:
* *Parylene PVD*

Process:
1. Deposit 10 microns of Parylene C on to wafers. [See Parylene C Coating Subprotocol]().
    1. 30-36 g of dimer is typical, but amount should be verified by comparing to past Parylene runs and adjusted as needed
    2. 12 wafers per batch is recommended and varying the wafer number will affect the amount of dimer required

### 1.3 Measure Parylene Thickness

Equipment:
* *Thin-film thickness measurement system*

Process: 
1. Measure Parylene thickness at center of wafer using non-contact optical profilometer
    1. As an alternative, glass reference slides can be coated alongside each Parylene C wafer shelf. Sections of the Parylene C coating on these slides can be removed by way of a sharp blade, and the reference slide coating thickness measured directly using a contact profilometer. Please note that this method is less accurate.
2. Log measurements into logbook

### 1.4 Thermal Anneal

Equipment:
* *Vacuum oven*

Process:
1. Anneal all wafers with base Parylene C at 150 °C under hard vacuum with a soak time of 4 hours. The purpose of the step is to improve thermal properties of the Parylene C prior to metal evaporation, and to improve adhesion of the Parylene C base to the carrier wafer prior to lithography in Step 2.

## 2. Electrode (Metal) Layer

### 2.1 Photomask Cleaning

_Note: This step should be skipped for newly purchased photomasks which have been first opened under cleanroom conditions_

_Safety: Use acid-resistant gloves, apron, and googles when using Nanostrip_

Materials:
* *Acetone*
* *Isopropanol*
* *Nanostrip*

Equipment:
* *Glass tank designated for Nanostrip*
* *Hotplate*
* *Mask tweezers*
* *Teflon mask holder*

Process:
1. Clean photomask prior to lithography. [See Photomask Cleaning Subprotocol]().

### 2.2 High Resolution Image Reversal Lithography

Materials:
* *5214-E Photoresist*
* *AZ340 Developer*
* *5 mL Polypropylene Syringe (per wafer)*
* *22-Gauge Luer Stub (per wafer)*

Equipment:
* *Vacuum oven with N<sub>2</sub>*
* *Contact mask aligner with UV source*
* *Photoresist spinner*
* *Hot plate*
* *IR temperature sensor*
* *UV intensity meter*
* *Wafer centering tool*
* HDPE trays for developer and water baths*
* *Wafer dipper/holding tool*
* *Contact profilometer*

Process:
1. Prepare an image reversal photoresist mask of the electrodes, traces, and contact pads. [See High Resolution Image Reversal Lithography Subprotocol]().
2. Confirm and record the thickness of the photoresist with contact profilometer. Target is 1.2 ± 0.15 micron.

### 2.3 Descum Wafer

_Note: this step should be performed immediately before metal deposition_

Equipment:
* *RIE*

Process:
1. Descum (clean) wafers in the RIE, two 4” wafers at the same time, using the following recipe:  
    150 mT, 100 W, 50 sccm O<sub>2</sub>, 180 s.

### 2.4 Deposit Metal

_Note: this step should be performed immediately after descum_

Materials:
* *Titanium*
* *Platinum*
* *Gold*

Equipment:
* *E-beam evaporator*

Process:
1. Coat the wafers in a layer of evaporated metal using e-beam evaporation.
    1. Metal stack and parameters:  
        20 nm Ti (1 Å/s)  
        25 nm Pt (1 Å/s)  
        155 nm Au (2 Å/s)  
        25 nm Pt (1 Å/s)

### 2.5 Pattern Metal via Lift-Off

Materials:
* *Acetone*
* *N-Methylpyrrolidone (NMP)*
* *Isopropanol*

Equipment:
* *Glass dishes designated for lift-off*
* *Sonicating bath*

Process:
1. Lift-off photoresist to reveal metal pattern. [See Metal Patterning via Lift-Off Subprotocol]().

### 2.6 Dry-Bake

_Note: this step should be performed immediately before Parylene C_

Equipment:
* *Vacuum oven with N<sub>2</sub>*

Process:
1. Bake wafers at 60 °C in an oven under light vacuum (35-40 cmHg) and N­<sub>2</sub> flow (15-20 sccm) for >15 minutes

## 3. Insulation Parylene C

### 3.1 Descum Wafer

Equipment:
* *Asher*

Process:
1. Descum (clean) wafers in the asher using the following recipe:  
    125 mT, 100 W, 30 sccm O<sub>2</sub>, 300 s

### 3.2 Silanization

_Note: this step should be performed within 12 hours of Parylene deposition_

Materials:
* *A-174 Silane*
* *Isopropanol*
* *Aluminum foil*

Equipment:
* *Glass dishes designated for A-174*
* *Crystalizing dish labeled for A-174*
* *Wafer cassette designated for A-174*
* *Stirring rod*

Process:
1. Treat the wafers with a solution of A-174 silane to improve adhesion to the insulating Parylene C layer. [See Silanization Subprotocol]().

### 3.3 Dry-Bake

_Note: this step should be performed immediately before Parylene C_

Equipment:
* *Vacuum oven with N<sub>2</sub>*

Process:
1. Bake wafers at 60 °C in an oven under light vacuum (35-40 cmHg) and N­<sub>2</sub> flow (15-20 sccm) for >15 minutes

### 3.4 Deposit Parylene C

_Note: this step should be performed within 12 hours after silanization_

Materials:
* *Parylene C Dimer*

Equipment:
* *Parylene PVD*

Process:
1. Deposit 10 microns of Parylene C on to wafers. [See Parylene C Deposition Protocol]().
    1. 30-36 g of dimer is typical, but amount should be verified by comparing to past Parylene runs and adjusted as needed
    2. 12 wafers per batch is recommended and varying the wafer number will affect the amount of dimer required

### 3.5 Measure Parylene Thickness

Equipment:
* *Thin-film thickness measurement system*

Process:
1. Measure Parylene thickness at center of wafer using non-contact optical profilometer
    1. As an alternative, glass reference slides can be coated alongside each Parylene C wafer shelf. Sections of the Parylene C coating on these slides can be removed by way of a sharp blade, and the reference slide coating thickness measured directly using a contact profilometer. Please note that this method is less accurate.
2. Log measurements into logbook

## 4. Pattern Parylene (Etch #1)

### 4.1 Photomask Cleaning

_Note: This step should be skipped for newly purchased photomasks which have been first opened under cleanroom conditions_

_Safety: Use acid-resistant gloves, apron, and googles when using Nanostrip_

Materials:
* *Acetone*
* *Isopropanol*
* *Nanostrip*

Equipment:
* *Glass tank designated for Nanostrip*
* *Hotplate*
* *Mask tweezers*
* *Teflon mask holder*

Process:
1. Clean photomask prior to lithography. [See Photomask Cleaning Subprotocol]().

### 4.2 Pattern Etch Mask with Photolithography

Materials:
* *12xt-20pl-15 photoresist*
* *MIF 726 developer*

Equipment:
* *Contact mask aligner*
* *Photoresist spinner*
* *Hot plate*
* *IR temperature sensor*
* *Wafer centering tool*

Process:
1. Prepare a photoresist etch mask, approximately 15 microns thick, defining the outline of the MEA, and the openings over the electrodes and contact pads. [See Etch Mask Lithography Protocol]().
2. Confirm and record the thickness of the photoresist with contact profilometer. Target is 16 ± 1 micron.

### 4.3 Etch Parylene

Equipment:
* *RIE-ICP or RIE*

Process:
1. Etch through approximately 10 microns of Parylene C using O<sub>2</sub> plasma using either deep reactive ion etch (DRIE) or reactive ion etch (RIE).
2. DRIE (preferred): A two-step switch-chemistry Bosch-type etch process using an ICP-RIE etching tool. Etch approximately 100-110 cycles in batches of 60 cycles or fewer, with wafers vented and cooled to room temperature between batches.
    1. Etch step:  
        Gas: 60 sccm O<sub>2</sub>, 40 sccm Ar  
        RF Power: 20 W  
        ICP Power: 700 W  
        Time: 10 seconds
    2. Passivation step:  
        Gas: 35 sccm C<sub>4</sub>F<sub>8</sub>, 40 sccm Ar  
        RF Power: 10 W  
        ICP Power: 700 W  
        Time: 3 seconds
    3. Etch rate: approximately 0.095 microns per loop
3. RIE (alternative): A single step O<sub>2</sub> RIE process. Two 4” wafers run side-by-side on a 10” platen.
    1. Gas: 50 sccm O<sub>2</sub>  
        RF Power: 150 W  
        Time: 50 minutes
    2. Etch rate: approximately 0.19 microns per minute.

### 4.4 Strip Photoresist Mask

Materials:
* *Acetone*
* *Isopropanol*

Equipment:
* *Glass dishes designated for photoresist stripping*
* *Solvent fume hood*

Process:
1. Perform chemical work in solvents fume hood
2. Soak wafer in acetone bath for 5 minutes.
3. Soak wafer in isopropanol bath for 5 minutes.
4. Soak in DI water for 5 minutes.
    1. 3× rinse in DI water
5. Blow dry with N<sub>2</sub>

### 4.5 Dry-Bake

_Note: this step should be performed immediately before Parylene C_

Equipment:
* *Vacuum oven with N<sub>2</sub>*

Process:
1. Bake wafers at 60 °C in an oven under light vacuum (35-40 cmHg) and N­<sub>2</sub> flow (15-20 sccm) for >15 minutes

## 5. Pattern Parylene (Etch #2)

### 5.1 Photomask Cleaning

_Note: This step should be skipped for newly purchased photomasks which have been first opened under cleanroom conditions_

_Safety: Use acid-resistant gloves, apron, and googles when using Nanostrip_

Materials:
* *Acetone*
* *Isopropanol*
* *Nanostrip*

Equipment:
* *Glass tank designated for Nanostrip*
* *Hotplate*
* *Mask tweezers*
* *Teflon mask holder*

Process:
1. Clean photomask prior to lithography. [See Photomask Cleaning Subprotocol]().

### 5.2 Pattern Etch Mask with Photolithography

Materials:
* *12xt-20pl-15 photoresist*
* *MIF 726 developer*

Equipment:
* *Contact mask aligner*
* *Photoresist spinner*
* *Hot plate*
* *IR temperature sensor*
* *Wafer centering tool*

Process:
1. Prepare a photoresist etch mask, approximately 15 microns thick, defining the outline of the MEA, and the openings over the electrodes and contact pads. [See Etch Mask Lithography Protocol]().
2. Confirm and record the thickness of the photoresist with contact profilometer. Target is 16 ± 1 micron.

### 5.3 Etch Parylene

Equipment:
* *RIE-ICP or RIE*

Process:
1. Etch through approximately 10 microns of Parylene C using O<sub>2</sub> plasma using either deep reactive ion etch (DRIE) or reactive ion etch (RIE).
    1. DRIE (preferred): A two-step switch-chemistry Bosch-type etch process using an ICP-RIE etching tool. Etch approximately 100-110 cycles without venting in between the process.
    2. Etch step:  
        Gas: 60 sccm O<sub>2</sub>, 40 sccm Ar  
        RF Power: 20 W  
        ICP Power: 700 W  
        Time: 10 seconds
    3. Passivation step:  
        Gas: 35 sccm C<sub>4</sub>F<sub>8</sub>, 40 sccm Ar  
        RF Power: 10 W  
        ICP Power: 700 W  
        Time: 3 seconds
    4. Etch rate: approximately 0.095 microns per loop
2. RIE (alternative): A single step O<sub>2</sub> RIE process. Two 4” wafers run side-by-side on a 10” platen.
    1. Gas: 50 sccm O<sub>2</sub>  
        RF Power: 150 W  
        Time: 50 minutes
    2. Etch rate: approximately 0.19 microns per minute.

### 5.4 Strip Photoresist Mask

_Note: Parylene C dies may begin to lift off from wafer during this step._

Materials:
* *Acetone*
* *Isopropanol*

Equipment:
* *Glass dishes designated for photoresist stripping*

Process:
1. Perform chemical work in solvents fume hood
2. Soak wafer in acetone bath for 5 minutes.
3. Soak wafer in isopropanol bath for 5 minutes.
4. Soak in DI water briefly (<2 minutes)
5. Carefully blow dry if possible

## 6. Release MEAs

_Note: Parylene C MEAs often curl following release due to inter-layer stress._

Equipment:
* *X-acto knife*
* *Miconeedles*
* *Sharp tweezers
* Stereoscope*

Process:
1. To remove a tabulated sheet:
    1. Place a droplet of water at the sheet edge.
    2. Looking through a stereoscope, use a scalpel or microneedle to gently lift the edge of the device, allowing the water to wick between the Parylene and the wafer
    3. If needed, tug very gently at the edge of the sheet or along a handling tab using tweezers.
        1. Add more water as needed

## 7. Post-Process Annealing

### 7.1 Release Stress (Flatten)

Materials:
* *Ceramic plates*
* *Isopropanol*

Equipment:
* *Hot plate*

Process:
1. Lay released MEAs flat on a ceramic plate. A few drops of isopropanol may help pull MEAs flat using surface tension.
2. Cover with second ceramic plate and place on hot plate.
3. Set hot plate to 115 °C. Wait 15 minutes after the hot plate has reached temperature and return to < 60 °C temperature. Allow plates and MEAs to cool on hot plate.

### 7.2 Vacuum Anneal

Materials:
* *Ceramic plates*

Equipment:
* *Vacuum oven with N<sub>2</sub>*

Process:
1. Sandwich released MEAs between clean ceramic plates and place in vacuum oven
2. Pump down vacuum oven, then rinse 3× with N<sub>2</sub>.
3. Anneal 200 °C with a soak time of 4 hours, and a ramp up/down time of 8 hours.

### 7.3 High Temperature Vacuum Anneal

Materials:
* *Ceramic plates*

Equipment:
* *Vacuum oven capable of reaching > 200 °C*

Process:
1. Sandwich released MEAs between clean ceramic plates and place in vacuum oven
2. Pump down vacuum oven.
3. Anneal 200 °C with a soak time of 4 hours, and a ramp up/down time of 8 hours.

## 8. Post-Process Cleaning

_Note: this step is recommended to remove any remaining scum on electrode sites and improve impedance values_

Materials:
* *Ceramic plates or glass plates/wafers*
* *Kapton tape*

Equipment:
* *Asher*

Process:
1. Attach released devices to a clean carrier wafer (Si or glass) with the electrode sites exposed using small pieces of Kapton tape
2. Clean devices in the Asher using the following recipe:  
    125 mT, 100 W, 30 sccm O<sub>2</sub>, 5 minutes
   
## A. Process Flow Diagram

![A diagram of a device pattern]

## B. Material Sources

_Note: Standard materials (e.g. acetone, DI water, cleanroom wipes, etc.) are not listed_

| **Material** | **Supplier** |
| --- | --- |
| CR-7 chrome etchant | Transene, Danvers, MA |
| Parylene dimer | Specialty Coating Systems, Indianapolis, IN |
| AZ 12XT-20PL-15 photoresist | AZ Electronic Materials, Branchburg, NJ |
| AZ 5214 E photoresist | AZ Electronic Materials, Branchburg, NJ |
| AZ 340 developer | AZ Electronic Materials, Branchburg, NJ |
| AZ 726MIF developer | AZ Electronic Materials, Branchburg, NJ |
| Edge Bead Removal (EBR) solvent | AZ Electronic Materials, Branchburg, NJ |
| NMP Rinse | AZ Electronic Materials, Branchburg, NJ |
| Titanium | Provided by USC cleanroom |
| Platinum | Provided by USC cleanroom |
| Gold | Provided by USC cleanroom |
| Nanostrip 2X | CMC Materials, Santa Ana, CA |

## C. Equipment Models

_Note: Standard equipment (e.g. tweezers, microscopes, N<sub>2</sub> gun, scale, etc.) are not listed_

| **Equipment** | **Model #** | **Supplier** |
| --- | --- | --- |
| Vacuum oven with N<sub>2</sub> | TVO-2 | Cascade Tek Inc., Longmont, CO |
| VO914A | Lindberg/Blue M, New Columbia, PA |
| Profilometer | DektakXT | Bruker, Billerica, MA |
| Spin coater | WS-400B-6NPP Lite | Laurell Technologies, North Wales, PA |
| Hot plate | PMC 730 Dataplate | Barnstead/Thermolyne, Dubuque, IA |
| 1000-1 | Electronic Micro Systems, Sutton Coldfield, UK |
| Sonicating bath | 3510 | Branson Ultrasonics, Danbury, CT |
| DRIE | Plasmalab 100 | Oxford Instruments, Bristol, UK |
| RIE | PlasmaPro 80 | Oxford Instruments, Bristol, UK |
| Series 85 | Technics, Pleasanton, CA |
| Asher | CV200RFS | Yield Engineering Systems, Fremont, CA |
| Mask aligner | Model 200 | OAI, San Jose, CA |
| E-beam evaporator | Mark 40 | CHA Industries, Livermore, CA |
| PRO Line PVD 75 | Kurt J. Lesker, Jefferson Hills, PA |
| Parylene PVD | PDS 2010 Labcoter | Specialty Coating Systems, Indianapolis, IN |
