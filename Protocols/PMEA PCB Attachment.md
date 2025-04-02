# Protocol: Packaging and Assembly of Parylene Microelectrode Arrays

Description: This document details the packaging and assembly protocol for connectorization of Parylene C microelectrode arrays (MEAs) with printed circuit board (PCB) connectors.

_Note: Standard equipment and materials (e.g. tweezers, microscopes, DI water, cleanroom wipes, N<sub>2</sub> gun, scale, etc.) are not listed in materials lists._

Table of Contents

1. [Printed Circuit Board (PCB) Preparation](#1-pcb-preparation)
   * [Separate, Sand, and Clean](#11-separate-sand-and-clean)
   * [Bump Contact Pads](#12-bump-contact-pads)
   * [Coin Contact Pads](#13-coin-contact-pads)
2. [Component/Connector Soldering](#2-componentconnector-soldering)
      * [Apply Solder Paste](#21-apply-solder-paste)
      * [Align and Attach Components](#22-align-and-attach-components)
      * [Reflow Solder](#23-reflow-solder)
      * [Clean PCB](#24-clean-pcb)
3. [Parylene C Coating](#3-parylene-c-coating)
      * [Mask Components](#31-mask-components)
      * [Deposit Parylene C](#32-deposit-parylene-c)
4. [Component Potting & Ground Attachment](#4-component-potting--ground-attachment)
      * [Pot Connectors](#41-pot-connectors)
      * [Demask](#42-demask)
      * [Solder Ground Wires](#43-solder-ground-wires)
5. [Polymer Ultrasonic on Bump (PUB) Bonding](#5-polymer-ultrasonic-on-bump-pub-bonding)
      * [Align MEA to PCB](#51-align-mea-to-pcb)
      * [PUB Bond MEA to PCB](#52-pub-bond-mea-to-pcb)
6. [Underfill & Overcoat](#6-underfill--overcoat)
      * [Underfill](#61-underfill)
      * [Overcoat](#62-overcoat)
<ol type="A">
  <li>     <a href="#a-material-sources">Material Source</a>   </li>
  <li>     <a href="#b-equipment-models">Equipment Models</a>   </li>
</ol>

## 1. PCB Preparation

### 1.1 Separate, Sand, and Clean
_Note: This section only applies to FR-4 PCBs_

Materials: 
* *400 grit sandpaper (or similar)*
* *Isopropanol*

Equipment: 
* *Ultrasonic cleaner*

Process:
1. Separate PCBs from panel.
2. Sand edges with 400 grit sandpaper.
   1. With sandpaper flat on desk or table, run PCB edges across sandpaper until smooth. Apply even force to keep edges flat.
3. Clean PCBs in ultrasonic cleaner.
   1. Isopropanol for 10 minutes
   2. DI water for 10 minutes
4. Blow dry with N<sub>2</sub>

### 1.2 Bump Contact Pads

Equipment: 
* *Ultrasonic wire bonder (ball type)*

Process:
1. Using a ball-bonder in bump mode, place two gold bumps, approximately 75 microns in diameter, on the center of each contact pad on the PCB.
    1. Bump parameters
   <br>Tool: Hybond Model 626
   <br>Gold wire: 1 mil
   <br>Capillary attachment: Small Precision Tools UTSDIC-38HH-AZM-1/16-19MM
   <br>Stage Temperature: 140 °C
   <br>Ultrasonic Power: 180 mW
   <br>Time: 180 miliseconds
   <br>Force: 12 grams
   <br>EFO Power: 29 arbitrary units
   <br>Pull Length: 02 units
   <br>Tail Length: 27 units
    <br>Loop Height: 010 units

2. For best results ensure PCB is flush with stage and held tightly by clamps and/or vacuum chuck. For flex-PCBs additional fixturing may be required. Above parameters are tailored for FR-4 and may need to be modified for flex-PCB.

### 1.3 Coin Contact Pads

Equipment: 
* *Ultrasonic wire bonder (ball or wedge type)*

Process:
1. Using an ultrasonic ball bonder or wedge bonder with a tape-automated-bonding (TAB) tool attachment flatten and level each gold bump into a ‘coin’. Each bump will be hit twice with the two separate settings below.
    1. Tool: Hybond Model 572a
   <br>Tab attachment: Small Precision Tools 7045W-C-9060-3/4-M
   <br>Stage Temperature: Room temperature  
   <br>Step #1:  
   <br>Ultrasonic Power: 3 units
   <br>Time: 4.4 units
   <br>Force: 5.0 units  
   <br>Step #2:  
   <br>Ultrasonic Power: 3.4 units
   <br>Time: 4.4 units
   <br>Force: 7.0 units

2. Resulting coins should be approximately 30 microns tall and 100 microns in diameter.

## 2. Component/Connector Soldering

### 2.1 Apply Solder Paste

Materials: 
* *Lead-free solder paste*
* *23-gauge Luer stub (4 mm in length)*

Equipment: 
* *Pneumatic fluid dispenser*
* *Stereoscope*

Process:
1. Remove solder-paste from refrigerator and allow to reach room temperature, approximately 20 minutes.
2. Connect solder-paste cartridge to fluid dispenser.
    1. Attach Luer stub
    2. Set dispenser to 15 PSI
3. With aid of stereoscope, apply a small dot of solder past to each solder pad. Paste should be dispensed in one motion for each pad.

### 2.2 Align and Attach Components

Equipment: 
* *Soldering iron*
* *Stereoscope*

Process:
1. With aid of stereoscope carefully place and align components onto solder pads.
    1. For components such as Omnetics connectors which often hang off the edge of the PCB, a spacer may be necessary.
2. With the soldering iron set to~650 °F solder a single outside leg of each component.
    1. If necessary, adjust alignment and solder a leg on the other side of the component.

### 2.3 Reflow Solder

Materials: 
* *Ceramic plate or stainless-steel tray*

Equipment:
* *Reflow oven*

Process:
1. Place PCBs to be soldered in stainless-steel tray or onto ceramic plate and place on reflow oven platform.
2. Solder components to PCB using reflow oven with following profile:
    1. Tool: DDM Novastar Model GF-B
   <br>Temperature: 240 °C
   <br>Time<sub>a</sub>: 90 seconds
   <br>Time<sub>b</sub>: 300 seconds

### 2.4 Clean PCB

Materials: 
* *Lead-free flux remover*
* *Isopropanol*

Equipment: 
* *Ultrasonic cleaner*

Process:
1. Descum (clean) wafers in the RIE, two 4” wafers at the same time, using the following recipe:  
    150 mT, 100 W, 50 sccm O<sub>2</sub>, 180 s.

## 3. Parylene C Coating

### 3.1 Mask Components

Materials:
* *PTFE tape*

Process:
1. Using thin PTFE tape, cover the bond pads, faces of all connectors, solder connectors for ground/reference wire attachment, and any other surface needed to be deinsulated
    1. PCB designs with vias may need to be masked on both sides to prevent Parylene C from diffusing through vias underneath masking tape.
    2. Tape must be snug; use tweezer, dental pick, or other small metal tool to firmly laminate tape over all surfaces.

### 3.2 Deposit Parylene C

Materials:
* *Parylene C dimer*

Equipment:
* *Parylene PVD*

Process:
1. Deposit 10 µm of Parylene C onto the PCBs. See Parylene C Deposition Protocol.
    1. 30 g of dimer is typical but will depend on number and size of PCBs.
    2. As Parylene C layer on PCBs cannot be measured directly, reference slides should be included in coating.
    3. PCBs should be placed on sheet of aluminum foil in coating system to prevent them from sticking to shelves.

## 4. Component Potting & Ground Attachment

### 4.1 Pot Connectors

Materials: 
* *Medical grade epoxy*
* *23-gauge Luer stub*
* *3 cc dispenser barrel*
* *Dispenser cap*

Equipment: 
* *Pneumatic fluid-dispenser*
* *Bell jar*
* *Scale*
* *Oven*

Process:
1. Weigh out and thoroughly mix components of medical grade epoxy.
    1. For Epotek MED-302-3M (preferred) the ratio is 10:4.5.
    2. 1-2 g is sufficient
2. Decant epoxy into dispenser barrel and degas in bell jar under vacuum for 1 hour
    1. Barrel should be capped and stood vertically to prevent epoxy from spilling or leaking
3. Connect barrel to fluid dispenser.
    1. Attach Luer stub
    2. Set dispenser to 15 PSI
4. Apply a thick layer of epoxy to all exposed component legs.
5. Cure in oven according to epoxy curing schedule
    1. For MED-302-3M this is 2 hours at 80 °C

### 4.2 Demask

Materials:
* *Isopropanol*
* *Razor or X-Acto knife*

Equipment: 
* *Ultrasonic bath*
* *Stereoscope*

Process:
1. Using a fresh razor blade or X-Acto knife remove the Parylene C insulation from the masking tape.
2. Soak the masking tape with isopropanol and gently remove the tape from contact pads and solder connections.
3. Clean PCBs in ultrasonic cleaner.
    1. Isopropanol for 5 minutes
    2. DI water for 5 minutes
    3. Blow dry with N<sub>2</sub>

### 4.3 Solder Ground Wires

Materials:
* *Fine, insulated, stainless-steel wires (0.003” bare, 0.0055” coated, annealed)*
* *Lead-free solder*
* *Stainless steel flux*
* *Micro swab*
  
Equipment: 
* *Soldering iron*
* *Stereoscope*
* *Micro scissors*

Process:
1. Cut 8-10 cm lengths of stainless-steel wire (typically 2 per PCB) and remove 1 cm of insulation from proximal end, and 3 cm from the distal end.
    1. Use stainless steel micro scissors to carefully strip insulation.
    2. Length and number of ground wire may vary with project design
2. Thread proximal end of wire through appropriate plated-through-hole on PCB. Bend de-insulated end to prevent wire from pulling out.
3. Using micro swab, apply small dab of stainless-steel flux to soldering site.
4. With soldering iron set to 650 °F, solder wire to board using lead-free solder.
5. Trim excess wire from underside of PCB.
6. Repeat as needed for each wire.

## 5. Polymer Ultrasonic on Bump (PUB) Bonding

### 5.1 Align MEA to PCB

Materials:
* *Adhesive tape*
  
Equipment: 
* *Stereoscope*

Process:
1. Place MEA face down over PCB contact pads.
2. Using stereoscope, align MEA to contact pads and secure in place with small pieces of tape.
    1. It is very important that the Parylene C MEA lies as flat as possible. If necessary small drops of isopropanol can be used to pull the MEA taught to the PCB using surface tension.

### 5.2 PUB Bond MEA to PCB

Equipment:
* *Ultrasonic wire bonder (ball or wedge type)*

Process:
1. Using an ultrasonic wire bonder with a tape-automated bonding (TAB) tool attachment, weld each contact pad on the Parylene MEA to the corresponding PCB pad, using the flattened gold coins as an intermediary. Each pad will be hit twice with the two separate settings below.
    1. Tool: Hybond Model 572A
   <br> Tab attachment: Small Precision Tools 7045W-TI-10050-3/4-M
   <br> Stage Temperature: Room temperature
   <br> Step #1:
   <br> Ultrasonic Power: 8.0 units
   <br> Time: 3.0 units
   <br> Force: 6.5 units
   <br>Step #2:
   <br> Ultrasonic Power: 9.0 units
   <br> Time: 4.5 units
   <br> Force: 6.0 units

    2.  Take all measures to try and keep the MEA laminated to the PCB

## 6 Underfill & Overcoat

### 6.1 Underfill

Materials: 
* *Medical grade epoxy (thin)*
* *32-gauge Luer stub*
* *3 cc dispenser barrel*

Equipment: 
* *Pneumatic fluid-dispenser*
* *Scale*
* *Stereoscope*
* *Oven*

Process:
1. Weigh out and thoroughly mix components of medical grade epoxy.
    1. For Epotek MED-301 (preferred) the ratio is 20:5
    2. 1 g is sufficient
2. Fill cartridge with epoxy and connect barrel to fluid dispenser.
    1. Attach Luer stub
    2. Set dispenser to 10 PSI
3. Apply small drops of epoxy to the edges/corners of the MEA and allow to underfill the space between the MEA and the PCB.
4. Allow to cure at room temperature (overnight) or in oven at 65 °C for 1 hour.

### 6.2 Overcoat

Materials: 
* *Medical grade epoxy*
* *23-gauge Luer stub*
* *3 cc dispenser barrel*
* *Dispenser cap*

Equipment: 
* *Pneumatic fluid-dispenser*
* *Bell jar*
* *Scale*
* *Oven*

Process:
1. Weigh out and thoroughly mix components of medical grade epoxy.
    1. For Epotek MED-302-3M (preferred) the ratio is 10:4.5
    2. 1-2 g is sufficient
2. Decant epoxy into dispenser barrel and degas in bell jar under vacuum for 1 hour
    1. Barrel should be capped and stood vertically to prevent epoxy from spilling or leaking
3. Connect barrel to fluid dispenser.
    1. Attach Luer stub
    2. Set dispenser to 15 PSI
4. Apply a thick layer of epoxy to entire surface of PCB
5. Cure in oven according to epoxy curing schedule
    1. For MED-302-3M this is 2 hours at 80 °C
6. Repeat on opposite side
7. Material Sources

_Note: Standard materials (e.g. isopropanol, DI water, cleanroom wipes, etc.) are not listed_

## A. Material Sources
| **Material** | **Model #** | **Supplier** |
| --- | --- | --- |
| Parylene C dimer |     | Specialty Coating Systems, Indianapolis, IN |
| Lead-free solder paste | 4900 P SAC305 | MG Chemicals, Burlington, Ontario, Canada |
| Lead-free flux remover | ES1697 | Chemtronics, Kennesaw, Georgia |
| Medical grade epoxy (thick) | MED-302-3M | Epoxy Technology, Billerica, MA |
| Medical grade epoxy (thin) | MED-301 | Epoxy Technology, Billerica, MA |
| Stainless-steel flux |     | Superior Flux & Mfg. Co., Cleveland, OH |
| Stainless-steel wire | 790900 | A-M Systems Inc., Sequim, WA |
| Dispenser barrel |     | North Richland Hills, TX |

## B. Equipment Models

_Note: Standard equipment (e.g. tweezers, microscopes, N<sub>2</sub> gun, scale, etc.) are not listed_

| **Equipment** | **Model #** | **Supplier** |
| --- | --- | --- |
| Ultrasonic wire bonder (ball type) | 626 | Hybond Inc., Escondido, CA |
| Ultrasonic wire bonder (wedge type) | 572A | Hybond Inc., Escondido, CA |
| Ball-bonder capillary | UTSDIC-38HH-AZM-1/16-19MM | Small Precision Tools, Petaluma, CA |
| TAB tool | 7045W-C-9060-3/4-M | Small Precision Tools, Petaluma, CA |
| 7045W-TI-10050-3/4-M |
| Pneumatic fluid-dispenser | Performus III | Nordson, Westlake, OH |
| Reflow oven | GF-B | DDM Novastar, Ivyland, PA |
| Parylene PVD | PDS 2010 Labcoter | Specialty Coating Systems, Indianapolis, IN |
