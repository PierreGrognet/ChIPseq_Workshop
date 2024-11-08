---
output:
  html_document: default
  pdf_document: default
use_math: true
---
# qPCR on ChIPed chromatin

The quality of the immunoprecipitated material is usually evaluated by qPCR before being converted into sequencing library. This is the aim of this section.




## Principle of the analysis: 

The Bio-Rad CFX Real-Time PCR detection system will be used with two pairs of primers that have been validated beforehand. All qPCR quantifications are done in triplicates.

Here we will use two pairs of primers:  

**> Pair A**<BR>
Primers FC77 (ctcccatcaaccccaagagc) and FC78 (gatggagacgtagaaggcgg)<BR>
Bind in the middle of Pa_2_11200 CDS, coding for **Actin**  

**> Pair B**<BR>
Primers FC125 (agctactgttgtcgtgctgg) and FC126 (tcgatgaagaatacggcggc)<BR>
Bind in the 5' region of a repressed gene (named Pa_5_80) surrounded with transposable elements



### Calculation of Amplification efficiency = primer efficiency

Below is an example of RAW data (output of CFX analysis software)

* B01/B02/B03, B04/B05/B06 and B07/B08/B09 are standard dilution (1:5 dilution ratio) of a DNA samples (three triplicates)
* Cq is given by the qPCR machine
* Cq Mean is the mean Cq of the three triplicates
* The log (Qty) correspond to the log value of the standard 

Using the RAW data, a standard curve can be plotted and the qPCR amplification efficiency calculated as follows:

<img src="Pictures/qPCR_RawData_StandardCurve.jpg" width="700">




### Calculation of "Percent of Input"

The "Percent of Input" is calculted using the Mean Cq value, primer efficiency and Input dilution. This is illustrated below for two primer pairs and 3 different IPs including one with a control GFP antibody.

<img src="Pictures/qPCR_Percent_Input_v2.jpg" width="700">




## Implementation for the practical

### Initial dilution of Input and ChIP-ed DNA

You can test different DNA dilutions to come across the right Cq (20-22) or do like me and test 1:5 which, in my opinion, correspondeds to a good approximation of the reality.

In theory, the measured Cq of the Samples should not differ from the ones of the Input by more than 4. The more the Cq differs, the less reliable are the quantifications. 




|<b>Figure -  Initial dilution of the INPUT and ChIP-ed material|
|:--:|
| ![dilution](Pictures/sample_dilution.JPG) |



### qPCR reactions to do

* Beforehand, we need to **quantify primer efficiency** for each pair of primers:
    + We need to prepare a "standard" by mixing different DNA as follows:
        - 1 volume of your diluted Input (12µL)
        - 0.5 volume of your diluted IP1 (6µL)
        - 0.5 volume of your diluted IP2 (6µL)
    + Make a serial dilution (1:5) this "standard" (5 µL into 20 µL H2O). 3 different dilutions are enough. *careful*: the acurracy of the serial dilution is essential.
    + These 3 dilutions are referred to as "std-1" (undiluted), "std-2" (1:5 dilution) and "std-3" (1:25 dilution) in the layout for the qPCR. 
    + These 3 dilution (= Standards) will be used to determine primer efficiency (see below).

|<b>Figure -  Standards preparation|
|:--:|
| ![Standards](Pictures/standards.JPG) |
    

### qPCR mix

Prepare a master mix for n+3 reactions (if you have 20 qPCR reaction to do, the mix should be prepared for 23 reactions)


* Each qPCR reaction is assembled as follow: 
    + 5μl of 2X MasterMix 
    + 2μl H2O 
    + 1μl of primer mix 5μM 
    + 2μl of diluted DNA


* How many qPCR wells per pair of students:
    + The three **standards**. In triplicates
    + A single **Input** diluted 1/5 (normally it's the same for each antibody but you can test them all before selecting one). In triplicates
    + All your **IP Samples** diluted 1/5 (or adequate dilution). In triplicates
    + Include **two Negative control wells** (i.e. wells in which DNA replaced by H2O)
    + [In some cases, we also need to PCR a **plate reporter point** (Known DNA concentration, always the same pair of primers between each plate) (optional: useful to compare samples on different runs).  We won't need it here.]

* In total, for each primer pair:
    - For the calculation of primer efficiency: 3 x 3 = 9 wells
    - negative controls (H2O): 2 wells
    - For the calculation of "Percent of Input": 3 wells Input + 3 wells IP1 + 3 wells of IP2 = 9 wells.
    - An optional "reporter point" (3 wells)


|<b>Figure -  Layout for the qPCR using 12-well strips|
|:--:|
| ![qPCR reactions](Pictures/qPCR_Reactions.jpg) |


|<b>Figure -  Layout for the qPCR using 8-well strips|
|:--:|
| ![qPCR reactions](Pictures/Layout_Plate_qPCR_8strips.png) |
    

## Analysis of the results:

* Once the RAW Cq data have been exported: 
    + Plot measured Cq as a function of the log10(quantity) of the 3 **standards**. This allows to determine qPCR efficiency (see above) and detect the presence of potential PCR inhibitors.
    + Determie the Percent of Input


* This and the rest of the analysis can be done using the provided excel file: [Excel file](qPCR_Analysis.xlsx)

* Formula:<BR>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<img src="Pictures/qPCR_formula.jpg" width="700">
    



**all the formulas will be explained during the workshop**
