# The evolution of cuticular hydrocarbon diversity in *Myrmecia* ant species
### Abstract
Cuticular hydrocarbons (CHCs) are one of the primary chemical cues in insects and play a essential role in nest-mate recognition in ants. However, while knowledge of the diversity and composition of CHC profiles in ants has significantly expanded, there is still little understanding on how patterns of chemical evolution have shaped CHC diversity between closely-related species (i.e. within a single genus). Unresolved questions include the extent to which such species have unique CHC profiles, and whether diversity has arisen through gradual accumulation of differences in chemical composition over evolutionary time, or through larger shifts in composition at speciation events. We investigated cuticular hydrocarbon diversity within the endemic Australian genus Myrmecia (bull ants),  examining the relationship of cuticular hydrocarbon profiles to phylogeny, and for one species (Myrmecia pilosula) the variation and relationship of CHC profile to geographic proximity.
Gas chromatography-mass spectrometry analysis was used to quantify CHC composition from 245 individual ants across 43 nests and 17 Myrmecia species. Permutational Analysis of Variance (PERMANOVA) was used quantify the relative amounts of variation between species and within species. Principal Components Analysis was used to identify differences in cuticular hydrocarbon profiles between species. Finally, Mantel tests were used to determine the relationships between phylogenetic distance and cuticular hydrocarbon profiles between species, and geographical distances and cuticular hydrocarbon profiles within M. pilosula. The PERMANOVA revealed that inter-species variation was over 30 times greater than intra-species variation, suggesting that CHCs are distinct and highly conserved within species, indicative of their potential role in inter-species recognition. A significant positive correlation was found between phylogenetic distance, and CHC profile chemical distances between species, suggesting that more closely related species have more similar cuticular hydrocarbon profiles, indicating a gradual mode of evolution following initial diversification between species. However, variation between nests with M. pilosula was also found to be significant, with each nest having its own unique cuticular hydrocarbon profile, suggesting that broader chemical profile differences can be found to originate even prior to species divergence. A weak (p = 0.07) positive trend was also observed between geographical distance and cuticular hydrocarbon profile distances between nest in M. pilosula, suggesting that differences may originate based on geographic separation or environmental cues.

### KEYWORDS
Ants, cuticular hydrocarbons, chemical communication, Myrmecia, signal evolution

# Repository contents
+ Complete *Myrmecia* phylogeny newick string file
+ Complete raw GC-MS output for all species used
+ R scripts for each analysis 

# R scripts overview

## 1. Weight x CHC output correlation R code
+ To determine if an individual ant's weight correlated with its overall CHC peak size output

## 2. PERMANOVA, PCA and Chemical distance matrix for all species' CHCs
+ ANOSIM and PERMANOVA to determine if there are significant differences between species' CHC profiles
+ PCA to visualise those differences between each species and each other species' CHC profile
+ Chemical distance matrix between each ant's CHC profile and each other CHC profile for the Mantel test

## 3. Create presence absence data and matrix
+ Convert any compound peak at over 0.5 in the dataset as present, and turn those distances into a matrix to determine if compound abundance affects differences between CHC profiles between species

## 4. Prune phylogeny and create phylogenetic distance matrix
+ Prune total genus phylogeney to only species used in this study, and create phylogenetic distances between each species and every other species for the mantel test

## 5. Mantel tests
+ For all species chemical distances x phylogenetic distances, and presence absence x phylogenetic distances to determine if CHc profiles are correlated with phylogenetic relationships

## 6. *Myrmecia pilsoula* PCA
+ Extract only *M. pilosula* results from GC-MS data, and conduct PERMANOVa and PCA to see differences in each nests' CHC profile
+ Create chemical distances matrix between each nest

## 7. *Myrmecia pilosula* geographic distance matrix and mantel test
+ Create distance matrix from *M. pilosula* data and conduct Mantel test with geographical and chemical distances to determine if CHC profiles are affected temporally.



