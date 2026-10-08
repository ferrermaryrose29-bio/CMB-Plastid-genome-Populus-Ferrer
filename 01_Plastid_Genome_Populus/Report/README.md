# CMB Plastid Genome: *Populus trichocarpa*

**Student:** [Mary Rose V. Ferrer]

**Course/Section:** Cell and Molecular Biology - [B]


This repository documents my laboratory activity on the plastid genome of *Populus trichocarpa* (black cottonwood, family Salicaceae), NCBI RefSeq accession **NC_009143.1** (157,033 bp, circular).

## Activities

| Activity | Description | Location |
|---|---|---|
| Characterization of a Plastid Genome | Genome retrieval from NCBI, Galaxy sequence statistics, gene and structure analysis, and the final report | `data/`, `results/`, `figures/`, `report/` |

## Selected Organism and Source
- **Genus:** *Populus*
- **Species:** *Populus trichocarpa*
- **Family:** Salicaceae
- **NCBI accession/version:** NC_009143.1 (RefSeq)
- **Database:** NCBI Nucleotide / RefSeq
- **Source link:** https://www.ncbi.nlm.nih.gov/nuccore/NC_009143.1
- **Date retrieved:** [September 29, 2026]
- **Associated reference:** Tuskan et al. (2006). The genome of black cottonwood, *Populus trichocarpa* (Torr. & Gray). Science 313(5793): 1596-1604.

## Plastome Summary
| Feature | Value |
|---|---|
| Genome size | 157,033 bp |
| GC content | 36.68% |
| Topology | Circular |
| LSC | 85,128 bp |
| SSC | 16,599 bp |
| IR (each copy) | 27,653 bp |
| Annotated gene features | 144 (counting IR copies) |
| Protein-coding (CDS) features | 98 |
| tRNA features | 37 |
| rRNA features | 8 |
| Pseudogene | 1 (*infA*) |

The region sizes add up to the full genome (85,128 + 16,599 + 2 × 27,653 = 157,033 bp). The LSC-IR-SSC-IR layout was worked out from the two inverted repeat entries in the GenBank record.

## How the Data Were Obtained
I searched NCBI Nucleotide for the *Populus* chloroplast complete genome and selected the RefSeq record NC_009143.1 for *Populus trichocarpa*. I confirmed that it was a complete circular genome and not a barcode gene or fragment. I downloaded the sequence in FASTA format and the annotated record in GenBank format, then uploaded the FASTA file to my own account at usegalaxy.org.

## Galaxy Analysis
- **History name:** Plastid_Populus_Ferrer
- **Dataset name:** Populus trichocarpa NC_009143.1
- **Datatype:** fasta
- **Tool used:** Fasta Statistics (summary stats)
- **Results:** 157,033 bp, 1 sequence record, GC content 36.68%, 0 N bases and 0 gaps
- **Screenshot:** `figures/galaxy_history_stats.png`

Galaxy reported a single sequence record, so the whole plastome is represented by one sequence.

## Summary of Gene Content and Observations
The GenBank record lists 144 gene features: 98 protein-coding, 37 tRNA, and 8 rRNA features plus one pseudogene (*infA*). These counts include genes in the inverted repeats, which are present twice; counting each IR copy once gives roughly 120 unique genes. All four rRNA genes (16S, 23S, 4.5S, 5S) lie in the IR and are duplicated. The annotation includes the photosystem genes (*psa*, *psb*), ATP synthase genes (*atp*), cytochrome b6f genes (*pet*), *rbcL*, RNA polymerase genes (*rpo*), ribosomal protein genes (*rpl*, *rps*), the *ndh* genes, and others such as *matK*, *clpP*, *accD*, *cemA*, and *ycf1* to *ycf4*.

Eleven protein-coding genes have introns: *atpF*, *clpP*, *ndhA*, *ndhB*, *petB*, *petD*, *rpl16*, *rpl2*, *rpoC1*, *ycf3*, and *rps12* (trans-spliced, with its first exon in the LSC and the other two exons in the IR). Several tRNA genes also contain introns, including tRNA-Lys (*trnK*) and tRNA-Ala (*trnA*).

GC content varies by region: the IR is highest at 41.92%, the LSC is 34.47%, and the SSC is lowest at 30.54%. The high GC in the IR is consistent with the rRNA genes located there.

## Repository Structure
- `README.md` - project overview
- `data/` - source FASTA and GenBank files for NC_009143.1
- `results/` - `genome_summary.csv` and `gene_table.csv`
- `figures/` - Galaxy screenshot
- `report/` - final completed report

## Data Sources and References
- NCBI Nucleotide / RefSeq NC_009143.1: https://www.ncbi.nlm.nih.gov/nuccore/NC_009143.1
- Galaxy: https://usegalaxy.org/
- Tuskan, G.A., et al. (2006). The genome of black cottonwood, *Populus trichocarpa* (Torr. & Gray). Science 313(5793): 1596-1604.

## How to Repeat This Analysis
1. Open the NCBI link above and download the FASTA and GenBank files for NC_009143.1.
2. Sign in to usegalaxy.org, create a new history, and upload the FASTA file. Confirm the datatype is fasta.
3. Run Fasta Statistics on the uploaded dataset and record the length, number of sequences, and GC content.
4. Use the GenBank file to count genes by type and to find the LSC, SSC, and IR regions from the inverted repeat entries.
