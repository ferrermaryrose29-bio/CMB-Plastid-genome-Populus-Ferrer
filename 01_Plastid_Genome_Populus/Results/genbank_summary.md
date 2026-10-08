# GenBank File Summary

## File Information

| Item | Value |
|---|---|
| File | `Populus_trichocarpa_NC_009143_1.gb` |
| Organism | *Populus trichocarpa* (Salicaceae) |
| Accession | NC_009143.1 (RefSeq) |
| Source | https://www.ncbi.nlm.nih.gov/nuccore/NC_009143.1 |
| Locus / version | NC_009143 / NC_009143.1 |
| Definition | *Populus trichocarpa* chloroplast, complete genome |
| Molecule / topology | DNA, circular |
| Length | 157,033 bp |
| Record date | 03-APR-2023 |
| BioProject | PRJNA927338 |
| Organelle / taxon | plastid:chloroplast / taxon 3694 |
| Lineage | Eukaryota; Viridiplantae; Magnoliopsida; Malpighiales; Salicaceae; *Populus* |
| File size | 320,839 bytes |

## Feature Counts

| Feature type | Count |
|---|---|
| gene | 144 |
| CDS | 98 |
| tRNA | 37 |
| rRNA | 8 |
| pseudogene (*infA*) | 1 |
| repeat_region (inverted repeats A and B) | 2 |
| source | 1 |

The 144 gene features are 98 CDS + 37 tRNA + 8 rRNA + 1 pseudogene.

## Genome Structure

| Region | Coordinates | Size | GC content |
|---|---|---|---|
| LSC | 1..85,129 | 85,129 bp | 34.47% |
| IRb | 85,130..112,781 | 27,652 bp | 41.92% |
| SSC | 112,782..129,381 | 16,600 bp | 30.54% |
| IRa | 129,382..157,033 | 27,652 bp | 41.92% |
| **Total** | 1..157,033 | **157,033 bp** | 36.68% |

The IR coordinates come from the two `repeat_region` entries.

## Gene Distribution (all copies, by start position)

| Feature | LSC | IR (both copies) | SSC | Total |
|---|---|---|---|---|
| CDS | 63 | 24 | 11 | 98 |
| tRNA | 22 | 14 | 1 | 37 |
| rRNA | 0 | 8 | 0 | 8 |

## Unique Genes (each IR copy counted once)

| Category | Count |
|---|---|
| Protein-coding (CDS) | 85 (76 named + 9 hypothetical ORFs) |
| tRNA | 30 |
| rRNA | 4 |
| Pseudogene | 1 (*infA*) |
| **Total** | **120** |

## Protein-Coding Genes by Group

| Group | Count | Genes |
|---|---|---|
| Photosystem I | 5 | *psaA*, *psaB*, *psaC*, *psaI*, *psaJ* |
| Photosystem II | 15 | *psbA*-*psbF*, *psbH*-*psbN*, *psbT*, *psbZ* |
| ATP synthase | 6 | *atpA*, *atpB*, *atpE*, *atpF*, *atpH*, *atpI* |
| Cytochrome b6f | 6 | *petA*, *petB*, *petD*, *petG*, *petL*, *petN* |
| RuBisCO | 1 | *rbcL* |
| RNA polymerase | 4 | *rpoA*, *rpoB*, *rpoC1*, *rpoC2* |
| NADH dehydrogenase | 11 | *ndhA*-*ndhK* |
| Ribosomal proteins (large) | 8 | *rpl2*, *rpl14*, *rpl16*, *rpl20*, *rpl22*, *rpl23*, *rpl33*, *rpl36* |
| Ribosomal proteins (small) | 11 | *rps2*, *rps3*, *rps4*, *rps7*, *rps8*, *rps11*, *rps12*, *rps14*, *rps15*, *rps18*, *rps19* |
| Other conserved genes | 9 | *matK*, *clpP*, *accD*, *cemA*, *ccsA*, *ycf1*, *ycf2*, *ycf3*, *ycf4* |
| Hypothetical ORFs | 9 unique (15 with IR copies) | labeled "hypothetical protein" |

## RNA Genes

| Type | Features | Unique | Notes |
|---|---|---|---|
| rRNA | 8 | 4 | 16S, 23S, 4.5S and 5S; all in the IR (two copies each) |
| tRNA | 37 | 30 | 14 tRNA features lie in the IR (7 duplicated genes) |

## Genes with Introns

| Type | Genes |
|---|---|
| Protein-coding (11) | *atpF*, *clpP*, *ndhA*, *ndhB*, *petB*, *petD*, *rpl16*, *rpl2*, *rpoC1*, *ycf3*, *rps12* (trans-spliced) |
| tRNA (6) | *trnK*, *trnA*, and the Gly, Ile, Leu and Val tRNAs |

## IR-Duplicated Genes

| Type | Genes |
|---|---|
| rRNA | 16S, 23S, 4.5S, 5S |
| tRNA | 7 tRNA genes |
| Protein-coding | *rps7*, *ndhB*, *rpl2*, *rpl23*, *rps19*, *ycf2*, *rps12* (3' exons) |
| Hypothetical ORFs | 6 |

## Notable Features

| Feature | Detail |
|---|---|
| Pseudogene | *infA* (80,807..81,043, minus strand), similar to *Spinacia oleracea* initiation factor 1 |
| *rps12* | Trans-spliced: first exon in the LSC (70,463..70,576); 3' exons in the IR, annotated in both IR copies |
| *ycf1* (full length) | 1,822 aa, 125,620..131,088, at the SSC/IRa boundary |
| *ycf1* (fragment) | 601 aa, 111,075..112,880, at the IRb/SSC boundary; labeled "hypothetical protein" in the record |
| *rps16* | No *rps16* annotation in this record |

## Notes on Interpretation

| Point | Status |
|---|---|
| Gene counts | Include both IR copies unless stated as unique |
| Unique gene counts | My own tally, made by counting each IR copy once |
| *ycf1* fragment as a truncated *ycf1* copy | Interpretation, not an annotation in the file |
| *rps16* | Only reported as not annotated in this record; loss in Salicaceae not verified |
