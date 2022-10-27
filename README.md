# afmicrobes

This is the supplementary data page for: 
Bernard G, Greenfield P, Ragan MA and Chan CX (2018) k-mer similarity, networks of microbial genomes and taxonomic rank. mSystems 3: e00257-18.
https://doi.org/10.1128/mSystems.00257-18

This replaces the the original URL indicated in the paper, hosted on bioinformatics.org.au.

## Viewing of downloaded phylogenonic networks on your local computer

The overall dataset is available as a compressed file (AF_networks.zip) at https://dx.doi.org/10.14264/uql.2017.436

AF_networks.zip upon decompression contain the following four folders:
whole-genomes_net_k25: networks generated using distances derived from whole-genome sequences
rRNAs_net_k25: networks generated using distances derived from rRNA gene sequences
no_rRNAs_net_k25: networks generated using distances derived from chromosomal sequences with rRNA genes removed
plasmid_net_k25: networks generating using plasmid genome sequences

All networks presented in HTML files were generated using Javascript script, specifically the D3 library (https://d3js.org/). The display of these networks is dependent on the location of the associated files and the capability of the web browser to access them locally.

A network may not be displayed properly if the web browser cannot access local files when interpreting the HTML file. Please ensure that your browser allows access to local files on your computer (from local HTML files); this option is disabled by default in some browsers, e.g. Google Chrome and Firefox.

An example for a solution using Python3:

1. After extracting the files, on a terminal go to the directory where the `index.html` file is located, and run
`python -m http.server 8888 &`

2. On your web browser, go to
`localhost:8888`

This should load the `index.html` page and the associated dynamic figures appropriately.
