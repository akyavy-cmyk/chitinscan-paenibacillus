# chitinscan-paenibacillus
Python pipeline that downloads Paenibacillus genomes from NCBI, predicts genes, detects chitin-degrading enzymes (GH18, GH19, GH20, LPMO) with HMM profiles, and ranks strains by chitin-degradation potential.

# ChitinScan is a Colab-ready Python workflow for screening bacterial genomes for chitin-degrading capability. Starting from NCBI accession numbers, it automatically downloads the genomes, predicts protein-coding genes with pyrodigal, and searches them with pyhmmer against Pfam profiles for chitinases (GH18/GH19), β-N-acetylhexosaminidases (GH20), lytic polysaccharide monooxygenases (AA10), chitin-binding modules, and chitosanases (GH46).

The output is a genome-by-feature table, a transparent chitin-degradation score, a heatmap, and a ranking of strains. If phenotype labels are available, an optional logistic-regression model with leave-one-genome-out cross-validation can be trained. Developed and applied to 46 Paenibacillus genomes.
