---
output:
  word_document: default
  html_document: default
---
# ChIP protocol


## Preparation of mycelium

Culture
- Inoculate 6 Roux bottles of 100 ml of medium with a fresh mycelium (grown 1 or 2 days on M2 medium at 27°C).
- Incubate 62 hours in the dark at 27°C.

Fixation
- Filter the mycelium on gauze, rinse once with PBS at room temperature.
- Fix in 100ml of PBS 1X + 2.5 ml Formaldehyde 37%, shake 15 min at 27°C. _Careful: Formaldehyde is toxic, work with appropriate safety equipements (gloves, chemical hood)_
- Stop with 2.5 ml of Glycine 2.5 M (shake for 5 min).

Grinding and storage (In cold room)
- Filter the mycelium (_the flow-through needs to be discarded in appropriate liquid trash bin_)
- Wash twice with cold PBS
- Dry on wattman paper (do not hesitate to press the mycelium)
- Grind with liquid nitrogen with mortar and pestle.  _Careful: Use appropriate safety equipments_
- Weight and store at -80°C in 50 mL Falcon tubes (transport in liquid nitrogen).

 

### Day 1

#### Lysis and chromatin digestion 

- In the cold room : Weigh approximately 200 mg of mycelium (cool the spatula in liquid nitrogen before each sample, no more than 2 samples after removal of the mycelium from liquid nitrogen)
- In the ice: Resuspend the mycelium with 1 mL of [Lysis buffer](Lysis_Buffer.md) (+proteinase inhibitor + CaCl2)
- Mix well 10 times going back and forth with the P1000, vortex, leave 10 min on ice, vortex again.
- Add 5μl of Micrococcale Nuclease and incubate 20-30 min at 37°C (in the water bath) (+ a control without MNase to check digestion), 
- Gently mix the tubes every 2 min to resuspend the mycelium.
- Stop the reaction with 30 μl of EGTA pH 8 0.5 M , incubate 5 min on ice.
- Centrifuge 3-5 min at 4°C at top speed, 
- Recover the supernatant (= soluble chromatin), 
- Repeat the centrifugation to remove as much as possible the undigested genomic DNA.
- Quantify the 2µL and 5µL of your chromatin (with [QuBit](QuBit.md), following the QuBit kit protocol). You may need to dilute an aliquot of the chromatin beforehand.

(Possibility of storing -80 ° C at this stage, but for the ChIP it is better to avoid the thawing steps).


#### Checking of chromatin fragmentation (nucleosomal digestion pattern)


* Save a 50µL aliqot of Micrococcale digested chromatin in a fresh tube, then add:
     + RNAse A (20mg/ml) 10 μl, 60 min at 37°C
     + Proteinase K (20mg/ml) 10 μl, 120 min at 65°C
     + SDS to 0.5% 
     + Incubate at 65°C over night to reverse the crosslink





### Day 2

#### Phenol extraction of the DNA


To the tube kept over-night at 65°C, 

* Adjust the volume to 300 µl with H2O
* Add 300μl phenol-chloroform  (**Carefull! Phenol and chloroform must be used under the fume hood!**)
* mix or vortex, 
* centrifuge 3 min (top speed, room temperature)
* recover the aqueous phase in a fresh tube
* Add 300 μl chloroform to the aqueous phase
* centrifuge 3 min (top speed, room temperature)
* recover the aqueous phase in a fresh tube


#### Ethanol precipitation:


+ Add 1/100th of glycogen
+ Add 1/10th Sodium Acetate 3 M. Mix
+ Add 2.5 volume of Ethanol 100%
+ Centrifuge 10 min 16000g, 4°C, carefully remove the supernatant without aspirating the pelet.
+ Add 500 μl cold ethanol 70% 
+ Centrifuge 10 min 16000g, 4°C, carefully remove the supernatant without aspirating the pelet.
+ Air dry for 10-20 min
+ Resuspend in 50 μl H2O
+ Load 10μl (+ 2μl of loading buffer) on a 1.5% agarose gel. Run 40 min at 50V.



It should looks like this:
<img src="Pictures/chromatin_ladder.png" width="400" height="500">
 

 


 

 

## ChiP:

Dilution the chromatin : 

- If needed, thaw the chromatin on ice.
- Seed 5µg of chromatin in a fresh tube. Adjust the volume to 1.1 ml with  cold [Lysis buffer](Lysis_Buffer.md) + protease inhibitor. Keep the tube on ice.

**Prepare as many tubes as necessary for the different IPs and controls you will need**


In the cold room:

- Pre-clearing: Wash 30µL of magnetic beads per IP, as instructed [here](reagents.md). Then add 30 μl of washed magnetic beads to the chromatin. Incubate between 1 hour and 4 hours at 4°C on a rotating wheel.
- Place the tubes on a magnetic rack for 2-3 min and recover the supernatant in a fresh tube. Keep the tube on ice.
- Save 100 μl (= Input) to a new tube and freeze it at -20°C or -80°C.
- Add the appropriate amount of antibody (see [here](reagents.md)) to the rest (1 ml). Incubate over night at 4°C on a rotating wheel.

 

**Caution**: 1 Tube (5μg) = 1 Precipitation with 1 antibody. Prepare 1 tube for each replicate of each antibody.

 
 
 

### Day 3

#### Binding and washes

- Wash 20µl of magnetic beads per IP, as instructed [here](reagents.md). Then add 20μl of washed magnetic beads to each IP and incubate 4h at 4°C on a rotating wheel.

- Washes: Place the eppendorf tube on the magnetic rack for 3 min, remove supernatant, add 1 ml of the following cold buffers and incubate 10 min on rotating wheel each time at 4°C.
    1. [Lysis buffer](Lysis_Buffer.md) without protease inhibitor without CaCl2 - x2
    2. [Lysis buffer NaCl](Lysis_Buffer_500.md)
    3. [LiCl Washbuffer](LiCl_Buffer.md) - x2
    4. [Tris-EDTA](Tris_EDTA.md)



#### Elution
- Resuspend the beads in 62.5μL of [TES](TES.md) preheated at 65°C and incubate at 65°C for 10 min (vortex every 2 min or shake with the thermomixer).
- Place the tube on magnet and Save the the supernatant in a DNA LoBind Tube.
- Repeat the elution with fresh TES, pool the two elutions into the same tube.


#### Cross-link reversal
- Adjust the volume of Input and Samples to 500 µL with [TES](TES.md).
- Incubate the Elution sample and the Input at 65°C over night to reverse the cross-link




### Day 4

#### DNA Purification

* Add 125 μl H2O to the Samples ------📝🔴----- *Benoit: 4/07/2022: needed? Remove? Update phenol/chloroform below if removed.* ------📝-----

* Treat the Input and Elution samples with:

     + RNAse A (20mg/ml): **2 μl for the Samples, 5 µl for the Inputs**, 120 min at 50°C
     + Proteinase K (20mg/ml): 10 μl, 120 min at 50°C
     + Add SDS to 0.5% ------📝🔴----- *Benoit: 4/07/2022: TES is already at 1% SDS. Remove?* ------📝-----


* Phenol extraction: to the Input and Elution Samples

     + Add: 500μl phenol-chloroform
     + mix or vortex, 
     + centrifuge 3 min (top speed at room temperature)
     + recover the aqueous phase in a fresh DNA LoBind tube
     + Add: 500 μl chloroform
     + centrifuge 3 min (top speed at room temperature)
     + recover the aqueous phase in a fresh DNA LoBind tube


#### DNA Precipitation

* To the Elution and Input:

  + Add 1/100th of glycogen
  + Add 1/10th of Sodium Acetate 3M
  + Vortex
  + Divide into two DNA LoBind tubes (approx 250µL / tube)
  + Add 2.5 volumes Ethanol 100% (i.e. approx 625µL 100% EtOH).
  + Centrifuge 10 min 16000g, 4°C, carefully remove supernatant without disturbing the pellet
  + Wash with 70% ethanol
  + Air dry 10-20 min
  + Resuspend each pellet in 15μl of [Tris-EDTA](Tris-EDTA.md). Combine the two pellets of the same IP together. Combine the two pellets of the Input together. The total volume is 30µL.


* Quantify 2µL of the Input and IP sample with the Qubit dsDNA HS kit (follow the [QuBit protocol](QuBit.md))

* Store at -20°C. Evaluate the IP specificity per qPCR and/or proceed with the library preparation.

