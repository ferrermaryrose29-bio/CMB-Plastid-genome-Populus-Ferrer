# Visualize Plastid Genome Structure

**Name:** Mary Rose V. Ferrer
**Course:** Cell and Molecular Biology, B

## Genome Information
| Item | Value |
|---|---|
| Scientific name | *Populus trichocarpa* (black cottonwood) |
| Family | Salicaceae |
| NCBI accession | NC_009143.1 (RefSeq) |
| Plastid genome length | 157,033 bp (circular) |
| Source of genome file | NCBI Nucleotide, record "Populus trichocarpa chloroplast, complete genome", downloaded in GenBank (full) format: https://www.ncbi.nlm.nih.gov/nuccore/NC_009143.1 |
| Original file | `data/Populus_trichocarpa_NC_009143.1.gb` (unchanged) |

This is the same plastid genome I used in the previous plastid genome activity.

## Software
OGDRAW (OrganellarGenomeDRAW), CHLOROBOX, Max Planck Institute of Molecular Plant Physiology: https://chlorobox.mpimp-golm.mpg.de/OGDraw.html
Reference: Greiner S, Lehwark P, Bock R. 2019. OrganellarGenomeDRAW (OGDRAW) version 1.3.1. Nucleic Acids Research 47: W59-W64.

## OGDRAW Settings Used
- Standard map mode
- Uploaded the annotated GenBank file
- Map type: Circular
- Sequence source: Plastid
- Inverted repeats: automatic detection
- GC content graph: drawn
- Direction of transcription: shown
- Legend: full legend
- Intron-containing genes marked with an asterisk: [CHECK: selected / not available]
- Output format: PNG

## Plastid Genome Map
![Plastid genome map](Screenshots/Populus_trichocarpa_plastid_map.png)

## Main Structural Features
The *P. trichocarpa* plastid genome is a circular 157,033 bp molecule with the usual quadripartite structure. A large single-copy region (LSC, 85,129 bp) and a small single-copy region (SSC, 16,600 bp) are separated by two inverted repeats (IRb and IRa, 27,652 bp each). Genes are found on both strands. Photosynthesis genes such as psbA, rbcL and psaA are in the LSC, and most ndh genes are in the SSC. The IRs carry all four rRNA genes, several tRNA genes, and protein genes such as rpl2, rpl23, ycf2, ndhB and rps7, which therefore appear twice on the map. The GC graph is not uniform. Region averages from my earlier analysis are LSC 34.47%, SSC 30.54% and IR 41.92%.

## Repository Contents
- `README.md`: this file
- `data/Populus_trichocarpa_NC_009143.1.gb`: original GenBank file
- `figures/Populus_trichocarpa_plastid_map.png`: OGDRAW map
- `answers/Lab_plastid_genome_answers.md`: answers to Questions 1-10 ([view answers](answers/Lab_plastid_genome_answers.md))
