# Almeida BK, Hawkes CV. Fungal SynCom Assembly and Impacts on Wheat Drought Response
Data and associated analyses for Almeida &amp; Hawkes MATRIX 2023 growth chamber experiment testing Fungal Priority and Diversity effects on wheat drought stress response

## Supplementary Data and Analysis

## Author Contact Information
Christine Hawkes
112 Derieux Place, Thomas Hall, North Carolina State University, Raleigh, NC 27607
chawkes@ncsu.edu

Mara DeMers
mara.demers@southeastmn.edu

Brianna Almeida
brianna.k.almeida@gmail.com

## Experiment Description
Triticum aestivum (AGS2000) was grown with fungal synthetic communities to investigate how fungal assembly mechanisms (priority, diversity) impacted the plants response to drought. All fungi were ascomycetes isolated from wheat fields from 7 fields across North Carolina. The communities contained a single pioneer fungus applied first, followed by low diversity (3 fungi) or high diversity (9 fungi) community inoculations. We imposed drought and measured plant growth and physiological performance.  Plants were grown in microcosms to prevent cross-contamination between fungal treatments. Treatments were replicated 6 times, including controls of sterile water. Prior to harvest, we measured height, leaf dieback, stomatal conductance, and severity of disease symptoms if there were any lesions present on the plants. After harvest we measured dry shoot and root mass. Final fungal community composition was assessed from leaf tissue with amplicon sequencing to understand synthetic community persistence and its impact on plant performance. 

## File list
AllMergedconcat.seq  
Almeida_FinalComAnalysis.Rmd  
Almeida_FinalComAnalysis.pdf  
Almeida_PlantPerformance.Rmd  
Almeida_PlantPerformance.pdf  
Almeida_NetworkAnalyses.pdf  
Almeida_NetworkAnalyses.Rmd  
Total_Harvest_Data.csv  
Total_Phys_Data.csv  
TraitsAndPersistence.csv  
best_matches.csv  
denovo_treeWNovSamples.nwk  
ForCompositionBarGraph.csv  
match_list_field_its.csv  
netcomi_filtered_assocMatrix.csv  
netcomi_filtered_edgelist.csv  
netcomi_filtered_nodelist.csv    
otu_cluster_column_cutoff1.csv  
otu_final.csv  
otu_final2.csv  
otu_table_for_cooccurence.csv    
phydist_2023_12_12.rds   
plotPerformance_backtransformed.csv   
presence_absence_OTUtable.csv  
presence_absence_otu_table_for_heatmap.csv  
relative_abundance_for_heatmap.csv  


## File descriptions
AllMergedconcat.seq – FASTA file containing concatenated sequences of actin, beta tubulin, ITS, LSU, and transcription factor 1 for each fungal isolate in the experiment and reference sequences acquired from the NCBI database

Almeida_FinalComAnalysis.Rmd and Almeida_FinalComAnalysis.pdf - R markdown script and knitted file for analyses related to final foliar community composition and graphing results

Almeida_PlantPerformance.Rmd and Almeida_PlantPerformance.pdf - R markdown script and knitted file for analyses of plant performance data and initial community inoculation and graphing results

Almeida_SelectingSynComs.Rmd  - R markdown script and knitted file for selecting synthetic community treatments based on phylogenetic distances 

Almeida_NetworkAnalyses.Rmd and Almeida_NetworkAnalyses.pdf - R markdown script and knitted file for analyzing field network characteristics and isolate persistence

best_matches.csv  - Best ASV matches from field wheat communities with fungi from synthetic community experiment
Variable|	Description|	Units|
| --- | --- | --- |
Mara_asv|	ASV id of fungi in field wheat communities|	NA
my_asv|	ASV or culture identity from sequenced synthetic communities|	NA
pct|	Percent overlap between ASV sequences|	NA

denovo_treeWNovSamples.nwk - Maximum likelihood tree created using RAxML 8 of fungi isolated from wheat. 

ForCompositionBarGraph.csv – presence/absence of initial synthetic community members at the end of the experiment as well as contaminant presence for graphing figures
Variable|	Description|	Units|
| --- | --- | --- |
Comm|	Combination of Pioneer, Diversity and Phylogenetic Treatment to indicate Community ID|	NA
Contam|	Indication is fungal isolate is a contaminant or not|	NA
Isolate|	Fungal isolate ID or Contaminant ID|	NA
Presence|	Is the isolate present in the community specified in Comm|	NA
Diversity| Diversity treatment, Low=4 taxa, High=10 taxa|	NA

match_list_field_its.csv - 

netcomi_filtered_assocMatrix.csv  

netcomi_filtered_edgelist.csv  

netcomi_filtered_nodelist.csv    

otu_cluster_column_cutoff1.csv  

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

presence_absence_OTUtable.csv – presence/absence data of samples (columns) by synthetic community isolates (labeled with numbers) and contaminants (rows) 

relative_abundance_for_heatmap.csv  

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

TraitsandPersistence.csv – Fungal trait performance
|Variable|	Description|	Units|
| --- | --- | --- |
sharedname|	Fungal| isolate ID|	NA
Persist|	Whether the isolate persisted to the end of the growth chamber experiment based on amplicon sequencing of the final foliar community|	NA
AverageNASlope| Average osmotic sensitivity of fungal isolates of those present at the end the end of the experiment for each fungal community treatment|	g/ g/NaCl/L
AverageIAA|	Average indole acetic acid production of fungal isolates in liquid media of those present at the end of the experiment for each fungal community treatment|µg/mL


## Note
## Publication Information
## Funding Information
This work was supported by the Tri Institutional Medical Mycology Training Fellowship (T32AI052080) and the Novo Nordisk Foundation (NNF19SA0059348) for funding.
## Additional data-raw sequences
Illumina Sequence data are available at the NCBI BioProject PRJNA1255089 and at the following NCBI Accessions.

| Isolate | Genus | ITS | LSU | Beta Tubulin | Actin | TEF1α |
|---------|-------|-----|-----|--------------|-------|-------|
| 03992 | *Didymella* | PZ167412 | PZ163016 | QB178706 | QB207368 | |
| 05501 | *Chaetosphaeronema* | PZ167398 | PZ162990 | | QB207349 | |
| 06070 | *Chaetosphaeronema* | PZ167403 | PZ162991 | | QB207351 | QB297733 |
| 06131 | *Didymella* | PZ167399 | PZ162992 | QB178685 | QB207342 | QB297725 |
| 06135 | *Mycosphaerella* | PZ167408 | PZ163017 | QB178705 | QB207371 | QB297752 |
| 06163 | *Didymella* | PZ167392 | PZ162993 | QB178681 | QB207341 | QB297727 |
| 06205 | *Didymella* | PZ167395 | PZ162995 | QB178684 | QB207347 | QB297730 |
| 06319 | *Chaetosphaeronema* | PZ167400 | PZ162989 | QB178689 | QB207348 | QB297732 |
| 06384 | *Didymella* | PZ167413 | PZ163018 | QB178708 | QB207366 | |
| 07778 | *Rosellinia* | PZ167409 | PZ163021 | QB178711 | | |
| 07999 | *Chaetosphaeronema* | PZ167415 | PZ163013 | QB178710 | | QB297750 |
| 11659 | *Stagonosporopsis* | PZ167416 | PZ163019 | QB178712 | QB207369 | |
| 13497 | *Mycosphaerella* | PZ167411 | PZ163022 | QB178707 | QB207367 | QB297749 |
| 13515 | *Chaetosphaeronema* | PZ167410 | PZ163014 | QB178704 | QB207365 | QB297748 |
| 13575 | *Didymella* | PZ167407 | PZ163015 | QB178713 | QB207370 | QB297751 |
| 13692 | *Didymella* | PZ167414 | PZ163020 | QB178709 | | |
| 13761 | *Didymella* | PZ167393 | PZ162994 | QB178683 | QB207344 | QB297728 |
| 16431 | *Didymella* | PZ167401 | PZ163011 | QB178686 | QB207343 | QB297729 |
| 16520 | *Cladosporium* | PZ167396 | PZ163012 | QB178687 | QB207345 | QB297731 |
| 16592 | *Epicoccum* | PZ167384 | PZ162983 | QB178698 | QB207359 | QB297743 |
| 16616 | *Nigrospora* | PZ167388 | PZ162984 | QB178702 | QB207363 | QB297746 |
| 16637 | *Epicoccum* | PZ167402 | PZ162985 | QB178690 | QB207350 | |
| 16704 | *Cladosporium* | PZ167394 | PZ162986 | QB178682 | QB207340 | QB297726 |
| 16772 | *Mycosphaerella* | PZ167404 | PZ162987 | | QB207352 | QB297734 |
| 16817 | *Boeremia* | PZ167397 | PZ162988 | QB178688 | QB207346 | |
| 19117 | *Mycosphaerella* | PZ167391 | PZ162996 | | QB207353 | QB297735 |
| 19298 | *Mycosphaerella* | PZ167378 | PZ162997 | QB178692 | | QB297738 |
| 19323 | *Cytospora* | PZ167381 | PZ162998 | QB178695 | | |
| 19488 | *Pyrenophora* | PZ167385 | PZ162999 | QB178699 | QB207360 | QB297744 |
| 19590 | *Daldinia* | PZ167390 | PZ163000 | | | QB297736 |
| 19593 | *Phaeosphaeria* | PZ167405 | PZ163001 | | | QB297737 |
| 21153 | *Xylaria* | PZ167387 | PZ163002 | QB178701 | QB207362 | |
| 21602 | *Cladosporium* | PZ167406 | PZ163003 | | QB207354 | |
| 21651 | *Xylaria* | PZ167386 | PZ163006 | QB178700 | QB207361 | QB297745 |
| 21710 | *Phaeosphaeria* | PZ167379 | PZ163004 | QB178693 | QB207355 | QB297739 |
| 21727 | *Xylaria* | PZ167382 | PZ163005 | QB178696 | QB207357 | QB297741 |
| 23958 | *Coniochaeta* | | PZ163007 | QB178691 | | |
| 24048 | *Nigrospora* | PZ167389 | PZ163008 | QB178703 | QB207364 | QB297747 |
| 24411 | *Nigrospora* | PZ167383 | PZ163010 | QB178697 | QB207358 | QB297742 |
| 24428 | *Pyrenophora* | PZ167380 | PZ163009 | QB178694 | QB207356 | QB297740 |

