# qPCR on ChIPed chromatin

Q-PCR mixture per well: 5μl of MasterMix 2μl H2O 1μl of primer mixture 5μM 2μl of diluted DNA

You can test different DNA dilutions to come across the right Cq (20-22) or do like me and test 1/20 which in my opinion corresponded to a good approximation of reality.

In theory the Cq of the Sample should not be different from more than a factor 4 of the Input, but for me I consider that we are OK if we stay in the range (avoid exceeding a Sample>30)

For each pair of primers tested:

-          Make a dilution range of 5 in 5 from a mixed of 1/20 DNA dilutions (Input+Sample), 3 points are enough. This curve makes it possible to determine the effectiveness of your primers and to detect if there are inhibitors.

-          Test an Input 1/20 (normally it's the same for each antibody but you can test them all before selecting one).

-          Test all Samples 1/20 (or adequate dilution)

-          Make 2 wells without DNA = negative controls

-          Make a plate reporter point (Known DNA concentration, always the same pair of antibodies between each plate)

Make each point in triplicat (=9 wells for the efficiency range + 2 neg control wells + 3 Input wells + 3 Sample wells x the number of duplicate ChiP x the number of antibodies tested + 3 reporter wells)

Analysis of the results:

Adjust the Cq of the imput (Imput=1/10 sample)

AdjustedCq= CalculatedCq-(ln(dilution factor)/ln(E))

 

Let CqInput be adjusted= Cq Inputcalculated-( ln(10)/ln(E)) if same dilution for Q-PCR

For each Sample:

%Input= E^(CqInput adjusted-CqSample)