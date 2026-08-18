# Almeida BK, Hawkes CV. Fungal SynCom Assembly and Impacts on Wheat Drought Response
Data and associated analyses for Almeida &amp; Hawkes MATRIX 2023 growth chamber experiment testing Fungal Priority and Diversity effects on wheat drought stress response

## Supplementary Data and Analysis

## Author Contact Information
Christine Hawkes
112 Derieux Place, Thomas Hall, North Carolina State University, Raleigh, NC 27607
chawkes@ncsu.edu

Brianna Almeida
112 Derieux Place, Thomas Hall, North Carolina State University, Raleigh, NC 27607
brianna.k.almeida@gmail.com

## Experiment Description
Triticum aestivum (AGS2000) was grown with fungal synthetic communities to investigate how fungal assembly mechanisms (priority, diversity) impacted the plants response to drought. All fungi were ascomycetes isolated from wheat fields from 7 fields across North Carolina. The communities contained a single pioneer fungus applied first, followed by low diversity (3 fungi) or high diversity (9 fungi) community inoculations. We imposed drought and measured plant growth and physiological performance.  Plants were grown in microcosms to prevent cross-contamination between fungal treatments. Treatments were replicated 6 times, including controls of sterile water. Prior to harvest, we measured height, leaf dieback, stomatal conductance, and severity of disease symptoms if there were any lesions present on the plants. After harvest we measured dry shoot and root mass. Final fungal community composition was assessed from leaf tissue with amplicon sequencing to understand synthetic community persistence and its impact on plant performance. 

## File list
AllMergedconcat.seq    
denovo_treeWNovSamples.nwk   
Almeida_FinalComAnalysis.Rmd   
Almeida_FinalComAnalysis.pdf   
Almeida_PlantPerformance.Rmd   
Almeida_PlantPerformance.pdf     
Total_Harvest_Data.csv     
Total_Phys_Data.csv     
plotPerformance_backtransformed.csv     
presence_absence_OTUtable.csv   
ForCompositionBarGraph.csv   
TraitsandPersistence.csv   
Almeida_FinalComAnalysis.Rmd   
Almeida_PlantPerformance.Rmd   

## File descriptions
AllMergedconcat.seq – FASTA file containing concatenated sequences of actin, beta tubulin, ITS, LSU, and transcription factor 1 for each fungal isolate in the experiment and reference sequences acquired from the NCBI database

denovo_treeWNovSamples.nwk -NWK tree file of AllMergedconcat.seq for calculating cophentic distances of synthetic community treatments

Almeida_FinalComAnalysis.Rmd and Almeida_FinalComAnalysis.pdf - R markdown script and knitted file for analyses related to final foliar community composition and graphing results

Almeida_PlantPerformance.Rmd and Almeida_PlantPerformance.pdf - R markdown script and knitted file for analyses of plant performance data and initial community inoculation and graphing results

Almeida_SelectingSynComs.Rmd and Almeida_SelectingSynComs.pdg - R markdown script and knitted file for selecting synthetic community treatments based on phylogenetic distances 


Total_Harvest_Data.csv- Plant responses and fungal trait measurements based on fungal community composition
Variable|	Description|	Units
| --- | --- | --- |
Plant|	Unique Plant Sample ID|	NA
AverageNA_Final|	Average osmotic sensitivity of fungal isolates of those present at the end the end of the experiment for each fungal community treatment|	g/ g/NaCl/L
SDNA_Final|	Standard deviation of osmotic sensitivity of fungal isolates of those present at the end the end of the experiment for each fungal community treatment|	
RangeNA_Final|	Range of osmotic sensitivity of fungal isolates of those present at the end the end of the experiment for each fungal community treatment	|
AverageIAA_Final|	Average indole acetic acid production of fungal isolates in liquid media of those present at the end of the experiment for each fungal community treatment|	µg/mL
SDIAA_Final|	Standard deviation of indole acetic acid production of fungal isolates in liquid media of those present at the end of the experiment for each fungal community treatment|	µg/mL
RangeIAA_Final|	Range of indole acetic acid production of fungal isolates in liquid media of those present at the end of the experiment for each fungal community treatment|	µg/mL
Microcosm|	Unique Microcosm ID|	NA
Comm|	Combination of Pioneer, Diversity and Phylogenetic Treatment to indicate Community ID|	NA
Pioneer|		Pioneer Treatment|	NA
Diversity Level|	Diversity treatment, Low=4 taxa, High=10 taxa|	NA
Phylogenetic Treatment|	Phylogenetic distance of the community with 3 indicating less distance and 1 indicating more distance|	NA
P.Div|	Combination of only Pioneer and Diversity treatments|	NA
Drought|	Drought treatment, D- means well-watered and D+ indicates drought|	NA
ExpectedTaxa|	How many isolates are expected to persist to the end of the experiment based on diversity treatment|	NA
ContamTaxaNum|	How many isolates that were contaminants based on amplicon sequencing of final leaf community|	NA
IsolateTaxaNum|	How many isolates from the initial inoculant was present based on amplicon sequencing of final leaf community| NA
TaxaNum|	Sum of ContamTaxaNum and IsolateTaxaNum|	NA
Tiller #|	How many tillers at the time of harvest|	NA
TotalLeaf #|	Sum of all leaves at the time of harvest|	NA
BrownLeaf #|	Total number of leaves with leaf tip browning, also referred to as leaf dieback|	NA
LesionLeaf|	Total number of leaves with lesions|	NA
Height|	Height of from the top of the soil to the tip of the plant|	cm
Ratio of lesion to total leaf|	Ratio of LesionLeaf to TotalLeaf #|	
Ratio of BrownToTotal|	Ratio of BrownLeaf # to the TotalLeaf #	|
TimeBlock|	ID of which time block that sample belongs to|	NA
Total_Shoot_Mass|	Total aboveground biomass|	g
Dry_Root_Mass|		Total belowground biomass| 	g
Total_Biomass_Data|	Sum of Total_Shoot_Mass and Dry_Root_Mass|	g
Root:Shoot|	Ratio of Total_Shoot_Mass to Dry_Root_Mass|	NA
IAA_of_Comm	Average| indole acetic acid production of fungal isolates in liquid media of those isolates that make up the fungal community treatment|	µg/mL
STDEV_ofIAA|	Standard deviation of indole acetic acid production of fungal isolates in liquid media of those isolates that make up the fungal community treatment|	µg/mL
Range of IAA|	Range of indole acetic acid production of fungal isolates in liquid media of those isolates that make up the fungal community treatment|	µg/mL
NASlope_of_Comm|	Average osmotic sensitivity of fungal isolates of those that make up the fungal community treatment|	
STDEV_ofNA|	Standard deviation of osmotic sensitivity of fungal isolates of those that make up the fungal community treatment|	
RangeofNA|	Range of osmotic sensitivity of fungal isolates of those that make up the fungal community treatment|	

Total_Phys_Data.csv – plant physiological performance data
Variable|	Description|	Units
| --- | --- | --- |
Plant Number|	Unique Plant Sample ID|	NA
Microcosm|	Unique Microcosm ID|	NA
Pioneer|	Pioneer Treatment|	NA
Diversity| Level	Diversity treatment, Low=4 taxa, High=10 taxa|	NA
Phylogenetic Treatment|	Phylogenetic distance of the community with 3 indicating less distance and 1 indicating more distance|	NA
Drought|	Drought treatment, D- means well-watered and D+ indicates drought|	NA
Comm|	Combination of Pioneer, Diversity and Phylogenetic Treatment to indicate Community ID|	NA
gsw|	Stomatal conductance|	mmol m⁻² s⁻¹
PhiPS2|	the effective quantum yield of Photosystem II|	NA
TimeBlock|	ID of which time block that sample belongs to|	NA

plotPerformance_backtransformed.csv – back transformations of transformed plant performance metrics for graphing  figures
|Variable|	Description	|Units|
| --- | --- | --- |
|Trait|	Which transformed plant performance metric this entry belongs|	NA
Drought |	Drought treatment, D- means well-watered and D+ indicates drought|	NA
avg|	Back transformed average|	NA
sd|	Back transformed standard deviation|	NA
se|	Back transformed tandard error|	NA
Ciup| Upper limit of the 95% confidence interval|	NA
Cidn|	Lower limit of the 95% confidence interval|	NA
Cuipdiff|	Ciup-avg|	NA
Cidndiff| Cidn-avg|	NA
Comm|	Combination of Pioneer, Diversity and Phylogenetic Treatment to indicate Community ID|	NA

TraitsandPersistence.csv – Fungal trait performance
|Variable|	Description|	Units|
| --- | --- | --- |
sharedname|	Fungal| isolate ID|	NA
Persist|	Whether the isolate persisted to the end of the growth chamber experiment based on amplicon sequencing of the final foliar community|	NA
AverageNASlope| Average osmotic sensitivity of fungal isolates of those present at the end the end of the experiment for each fungal community treatment|	g/ g/NaCl/L
AverageIAA|	Average indole acetic acid production of fungal isolates in liquid media of those present at the end of the experiment for each fungal community treatment|µg/mL

ForCompositionBarGraph.csv – presence/absence of initial synthetic community members at the end of the experiment as well as contaminant presence for graphing figures
|Variable|	Description|	Units|
| --- | --- | --- |
|Comm|	Combination of Pioneer, Diversity and Phylogenetic Treatment to indicate Community ID|	NA|
|Contam| Indication is fungal isolate is a contaminant or not|	NA
|Isolate|	Fungal isolate ID or Contaminant ID|	NA
|Presence|	Is the isolate present in the community specified in Comm|	NA
|Diversity|	Diversity treatment, Low=4 taxa, High=10 taxa|	NA

presence_absence_OTUtable.csv – presence/absence data of samples (columns) by synthetic community isolates (labeled with numbers) and contaminants (rows) 

## Note
## Publication Information
## Funding Information
This work was supported by the Tri Institutional Medical Mycology Training Fellowship (T32AI052080) and the Novo Nordisk Foundation (NNF19SA0059348) for funding.
## Additional data-raw sequences
Sequence data are available at the NCBI Sequence Read Archive (XX)
