# Chromatin Immunoprecipitation: Principle and available Antibodies


## Overview of ChIP protocol

**ChIP** stands for **Ch**omatin **I**mmuno**P**recipitation. This technique is used to determine whether specific protein (or specific protein modifications) are found at specific genomic regions. The overall goal is to **isolate all DNA regions bound to a specific protein** using **antibodies** recognizing the protein (or the modifiedf protein) of interest.

|<b>Figure -  Simplified representation of the ChIP-procedure.</b> <BR> Source: Pierre Grognet|
|:--:|
| ![ChIP protocol](Pictures/ChIP.png) |





It relies on the following key steps:

1. Many proteins bind to DNA (eg. transcription factors, histones, etc.). Before extracting the chromatin, covalent bound are created between DNA and proteins. This is called "cross-linking". The cross-linking is performed by treating the cells with PFA (paraformaldehyde).

2. After extraction, the chromatin is sheared into small fragments either by sonication or thanks to enzyme such as the Micrococcal nuclease.

3. An antibody raised against the protein of interest is added to the sheared chromatin...

4. ... and binds to its target (here, the orange protein).

5. We then add magnetics beads coated with proteins called Protein G or Protein A. These proteins are able to bind the constant part of IgG.

6. The magnetic beads bound to the chromatin-protein-antibody complex is precipitated with a magnet. They stay stuck to tube while the rest is discarded with the supernatant.

7. We separate the beads, proteins and DNA from each other (by heating).

8. The DNA is purified...

9. ... and can be used for: 
    - qPCR (ChIP-qPCR)
    - Sequencing (ChIP-seq)
    - Microarray (ChIP-on-Chip)
    - ...



    
## Targeted Proteins and histone marks

The following histones marks and protein will be targeted during this course. Please note that not every mark will be targeted every year.

Important informations about the antibodies are also in the table below.

| Target     | Supplier | Catalog Number | Lot Number   | Quantity per IP |
| ---------- |--------- | -------------- | ----------   | --------------- |
| H3K36me3   | Abcam    | ab9050         | GR3307136-2  | 10 µL           |
| H3K27me3   | Sigma    | 17-622         | 3504435      | 5µL             |
| H3K9me3    | Abcam    | ab8898         | GR3373564-1  | 3.75µL (=3.75µg)|
| H3K4me3    | ActiveMotif | 39159       | 31420006     | 4 µL            |
| H4K20me3   | ActiveMotif | 39671       | 35518005     | 7.5 µL          |
| RNA Pol.II | ActiveMotif | 91151       | 26520003     | 4 µL    (=4µg)  |
| GFP        | Abcam    | ab290          | GR3321614-1  | 3µL             |



