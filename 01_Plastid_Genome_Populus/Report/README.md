# Characterization of a Plastid Genome: *Populus trichocarpa*

**Name:** Mary Rose V. Ferrer
**Course:** Cell and Molecular Biology, B, Negros Oriental State University
**Genome retrieved:** September 29, 2026
**Galaxy history:** Plastid_Populus_Ferrer

## Summary Table

| Feature | Value |
|---|---|
| Species / family | *Populus trichocarpa* / Salicaceae |
| Accession | NC_009143.1 (RefSeq) |
| Genome size | 157,033 bp |
| GC content | 36.68% |
| Topology | Circular |
| LSC / IR / SSC / IR | 85,128 / 27,653 / 16,599 / 27,653 bp |
| Gene features (all copies) | 144 (98 CDS, 37 tRNA, 8 rRNA, 1 pseudogene) |
| Unique genes | About 120 (4 rRNA, about 30 tRNA, the rest protein-coding), counting each IR copy once. This is my own approximate count. |
| Other features | Hypothetical ORFs, 1 pseudogene (*infA*) |
| Introns | 11 protein-coding genes and 6 tRNA genes with introns |

Files: `data/` (FASTA and GenBank), `results/genome_summary.csv`, `results/gene_table.csv`, `figures/galaxy_history_stats.png`

## Questions

### 1. Organism, accession and size

The organism is *Populus trichocarpa* (black cottonwood), family Salicaceae. The NCBI accession/version is NC_009143.1, taken from NCBI Nucleotide (RefSeq). The complete plastid genome is 157,033 bp long.

### 2. Evidence that it is a complete plastid genome

- It is a RefSeq record (NC_ prefix) for the complete chloroplast genome of *P. trichocarpa*, not a barcode gene or a fragment.
- The GenBank record is annotated as circular and has the typical plastid features and gene set.
- Galaxy Fasta Statistics shows 1 sequence of 157,033 bp with 0 N bases and 0 gaps, so the whole genome is one continuous record.
- The sequence has the LSC-IR-SSC-IR layout, and its genes (photosystem, ATP synthase, *rbcL*, rRNA, tRNA, ribosomal proteins) are typical of plastids.
- A nuclear sequence would not be a 157 kb molecule made up almost entirely of conserved plastid genes.

### 3. Overall organization

Yes, it has the common quadripartite LSC-IR-SSC-IR arrangement. The IR coordinates come from the two repeat_region entries in the GenBank record, and the SSC lies between them.

| Region | Coordinates | Size |
|---|---|---|
| LSC | 1..85,128 | 85,128 bp |
| IRb | 85,129..112,781 | 27,653 bp |
| SSC | 112,782..129,380 | 16,599 bp |
| IRa | 129,381..157,033 | 27,653 bp |

The sizes add up to the full genome: 85,128 + 16,599 + 2 × 27,653 = 157,033 bp. The two IRs are inverted copies of each other and separate the two single-copy regions.

### 4. Gene content and IR duplication

The GenBank file lists 144 gene features: 98 CDS, 37 tRNA, 8 rRNA and 1 pseudogene (*infA*). These counts include the genes in both IR copies. When each IR copy is counted once, there are about 120 unique genes.

Genes in the inverted repeats appear in two copies because the IRa and IRb are duplicated sequences, so every gene inside them is annotated once for each copy. The duplicated genes include all four rRNA genes (16S, 23S, 4.5S, 5S), 7 tRNA genes, and the protein genes *rps7*, *ndhB*, *rpl2*, *rpl23*, *rps19* and *ycf2*, as well as the last two exons of *rps12*.

Protein-coding genes found by group:

| Group | Genes |
|---|---|
| Photosystem I | *psaA*, *psaB*, *psaC*, *psaI*, *psaJ* (5) |
| Photosystem II | 15 *psb* genes |
| ATP synthase | 6 *atp* genes |
| Cytochrome b6f | *petA*, *petB*, *petD*, *petG*, *petL*, *petN* |
| RuBisCO | *rbcL* |
| RNA polymerase | *rpoA*, *rpoB*, *rpoC1*, *rpoC2* |
| NADH dehydrogenase | 11 *ndh* genes |
| Ribosomal proteins | 8 *rpl* and 11 *rps* genes |
| Others | *matK*, *clpP*, *accD*, *cemA*, *ccsA*, *ycf1* to *ycf4* |

### 5. Protein-coding genes from different functional groups

| Gene | Group | Function |
|---|---|---|
| *psaA* | Photosystem I | Core reaction-centre protein of PSI |
| *psbA* | Photosystem II | D1 protein of the PSII reaction centre |
| *petB* | Cytochrome b6f | Cytochrome b6 subunit, electron transfer between PSII and PSI |
| *atpA* | ATP synthase | Alpha subunit of ATP synthase, which makes ATP |
| *rbcL* | RuBisCO | Large subunit of RuBisCO, fixes CO2 in the Calvin cycle |
| *rpoB* | RNA polymerase | Beta subunit of the plastid-encoded RNA polymerase |
| *rps7* | Ribosomal protein | Small ribosomal subunit protein used in translation |
| *ndhF* | NADH dehydrogenase | Subunit of the NDH complex, involved in cyclic electron flow |
| *matK* | Maturase | Helps splice group II introns |
| *clpP* | Protease | Catalytic subunit of the Clp protease |

### 6. RNA and RNA-processing features

- **rRNA genes:** *rrn16* (16S), *rrn23* (23S), *rrn4.5* (4.5S) and *rrn5* (5S). All four are in the IR, so there are 8 rRNA features in total.
- **tRNA genes:** 37 tRNA features in the record, for example *trnK* (tRNA-Lys), *trnA* (tRNA-Ala), and the tRNA-Gly, tRNA-Leu, tRNA-Val and tRNA-Ile genes.
- **Protein-coding genes with introns:** *atpF*, *clpP*, *ndhA*, *ndhB*, *petB*, *petD*, *rpl16*, *rpl2*, *rpoC1*, *ycf3* and *rps12*. *rps12* is trans-spliced: its first exon is in the LSC and its other two exons are in the IR.
- **tRNA genes with introns:** *trnK*, *trnA* and the Gly, Leu, Val and Ile tRNAs (6 in total).
- *matK* encodes a maturase that is thought to help splice group II introns.

### 7. Pseudogenes, duplications and unusual features

- **Pseudogene:** *infA* (80,807..81,043) is annotated as a pseudogene, similar to spinach initiation factor 1.
- **Duplications:** the IR duplicates the rRNA genes, 7 tRNAs, *rps7*, *ndhB*, *rpl2*, *rpl23*, *rps19*, *ycf2* and the *rps12* 3' exons.
- **Trans-splicing:** *rps12* is split between the LSC and the IR.
- **ycf1:** a full-length *ycf1* (1,822 aa) lies near the SSC/IRa boundary. A shorter 601 aa copy (111,075..112,880) at the IRb/SSC boundary is labeled "hypothetical protein" in the record. I think this is a truncated *ycf1* copy at the boundary, but that is my interpretation and not stated in the annotation.
- **rps16:** I could not find an *rps16* annotation in this record. Loss of *rps16* has been reported in some Salicaceae, but I did not verify that, so I am only reporting that it is not annotated here.
- No other rearrangements are noted in the record.

### 8. GC content and other observations

The GC content is 36.68% (Galaxy: 157,033 bp, 1 record, no Ns; A 49,158, T 50,283, C 29,304, G 28,288). Two other observations:

1. GC content differs by region: LSC 34.47%, SSC 30.54% and each IR 41.92%. The IR is highest, which fits with the GC-rich rRNA genes located there.
2. The two inverted repeats are 27,653 bp each, so together they make up about 35% of the whole genome, and the genome is divided into the four regions of the quadripartite structure.

### 9. Plastid vs. mitochondrial genome

**Five similarities**

1. Both come from bacterial endosymbionts (cyanobacteria for plastids, alpha-proteobacteria for mitochondria).
2. Both are DNA genomes found inside double-membrane organelles.
3. Both encode some rRNAs, tRNAs and proteins, but depend on nuclear-encoded proteins for most functions.
4. Both are usually inherited from the mother in most flowering plants, although this varies among lineages.
5. Both have lost or transferred many genes to the nucleus, and both contain introns.

**Five differences:** see the comparison table below (location, function, organization, size, gene content, copy number and recombination).

## Plastid vs. Mitochondrial Genome Comparison

| Feature | Plastid genome | Mitochondrial genome |
|---|---|---|
| Cellular location | Plastids (chloroplasts) | Mitochondria |
| Main biological functions | Photosynthesis and plastid gene expression | Respiration and ATP production |
| Typical genome organization | Usually one circular map with LSC, SSC and two IRs | Often large and multipartite, with recombining subgenomic forms |
| Relative genome size | Small and conserved (157,033 bp here) | Larger and highly variable in plants, from hundreds of kb to over a Mb |
| Gene content | About 110-130 genes: photosynthesis, rRNA, tRNA, ribosomal proteins | About 50-60 genes: respiratory complexes, ribosomal proteins, some tRNAs |
| Copy number | Very high, often hundreds to thousands per cell | Lower, tens to hundreds per cell |
| Inheritance | Mostly maternal in angiosperms (varies by lineage) | Mostly maternal (varies by lineage) |
| Recombination / structural change | Structure is conserved; IR-mediated recombination, rare rearrangements | Frequent recombination across repeats, rapid structural change |
| Mutation / substitution pattern | Low to moderate substitution rate, conserved sequence | Very low point mutation rate but fast rearrangement and uptake of foreign DNA |
| Common research applications | Phylogenetics, barcoding, plastid transformation, ancient and herbarium DNA | Cytoplasmic male sterility, breeding, genome-structure evolution |

### 10. Practical value, limitations and research questions

**Advantages compared with the nuclear genome**

- High copy number gives a high DNA yield and works with degraded or herbarium DNA.
- It is small, compact and conserved, so it is easy to sequence and assemble.
- It is mostly uniparental and does not recombine much, which gives a clear maternal lineage and simpler phylogenies.
- Conserved gene content allows universal primers and barcodes (*rbcL*, *matK*).
- It avoids the repeat-rich, large nuclear genome. Nuclear sex chromosomes (such as the sex-determining region of dioecious *Populus*) are repetitive, have restricted recombination and are harder to assemble.
- It can be used for plastid transformation and genetic engineering.

**Limitations**

- It is effectively one locus with one (usually maternal) history, so it cannot show paternal contribution, hybridization or introgression.
- Low variation may not separate closely related species. This matters in *Populus*, where hybridization is common.
- Plastid DNA copies that moved to the nucleus (NUPTs) can contaminate data.
- It carries no information about most nuclear traits such as sex determination or wood formation.

**Research questions**

- **Plastid data:** What is the maternal lineage and relationship among *Populus* species or populations?
- **Nuclear data:** Which genes control sex determination or wood formation in *Populus*, or how much introgression occurs between hybridizing species?

## References

- NCBI RefSeq NC_009143.1, *Populus trichocarpa* chloroplast, complete genome. https://www.ncbi.nlm.nih.gov/nuccore/NC_009143.1
- Tuskan, G.A., et al. (2006). The genome of black cottonwood, *Populus trichocarpa* (Torr. & Gray). Science 313(5793): 1596-1604.
- Galaxy (Fasta Statistics): https://usegalaxy.org/
