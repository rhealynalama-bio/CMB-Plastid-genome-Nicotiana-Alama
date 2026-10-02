# Characterization of a Plastid Genome: *Nicotiana tabacum*

**Name:** Rhealyn F. Alama

**Course:** Cell and Molecular Biology

**Genome retrieved:** September 29, 2026

**Galaxy history:** Plastid_Nicotiana_ALAMA

---

## Summary Table

| Feature | Value |
|---|---|
| Species / family | *Nicotiana tabacum* / Solanaceae |
| Accession | NC_001879.2 (RefSeq) |
| Genome size | 155,943 bp |
| GC content | 37.85% |
| Topology | Circular |
| LSC / IRb / SSC / IRa | 86,686 / 25,343 / 18,571 / 25,343 bp |
| Gene features (all copies) | 144 (98 CDS, 37 tRNA, 8 rRNA, 1 pseudogene) |
| Unique named genes | 112 (78 protein-coding, 30 tRNA, 4 rRNA) |
| Other features | 10 hypothetical ORFs, 1 pseudogene (infA) |
| Introns | 16 intron features in 12 genes |

(Full table: `results/plastome_summary_table.md`)

---

## Questions

### 1. Organism, accession and size
*Nicotiana tabacum* (common tobacco), family Solanaceae. NCBI accession/version
NC_001879.2, from NCBI Nucleotide (RefSeq). Complete plastid genome size: 155,943 bp.

### 2. Evidence that it is a complete plastid genome
- Title: "Nicotiana tabacum plastid, complete genome," and the record states
  `/organelle="plastid"` and `COMPLETENESS: full length`.
- It is a RefSeq record (NC_ prefix), derived from the published full sequence
  (Shinozaki et al., 1986).
- Galaxy Fasta Statistics shows 1 sequence of 155,943 bp with no Ns, so the
  whole genome is a single gap-free record, not a barcode gene or fragment.
- It is circular and has the LSC-IR-SSC-IR layout, and its gene content (photosystem,
  ATP synthase, rbcL, rRNA, tRNA, ribosomal protein genes) is typical of plastids.
- A nuclear sequence would not be 156 kb of conserved plastid genes.

### 3. Overall organization
Yes, it has the common quadripartite LSC-IR-SSC-IR arrangement:

| Region | Coordinates | Size |
|---|---|---|
| LSC | 1..86,686 | 86,686 bp |
| IRb | 86,687..112,029 | 25,343 bp |
| SSC | 112,030..130,600 | 18,571 bp |
| IRa | 130,601..155,943 | 25,343 bp |

The two IRs are identical, inverted copies that separate the two single-copy regions.

### 4. Gene content and IR duplication
The GenBank file lists 144 gene features: 98 CDS, 37 tRNA, 8 rRNA and 1
pseudogene. Counting each gene once, there are 112 named genes (78
protein-coding, 30 tRNA, 4 rRNA), plus 10 hypothetical ORFs and 1 pseudogene
(infA).

Genes in the inverted repeats appear in two copies because the IRa and IRb
are duplicated sequences, so each gene they contain is annotated once per
copy. These include the four rRNA genes, 7 tRNAs, ndhB, rpl2, rpl23, rps7,
rps12, ycf2 and four ORFs.

### 5. Eight protein-coding genes from different functional groups

| Gene | Group | Function |
|---|---|---|
| psaA | Photosystem I | Core reaction-centre protein of PSI |
| psbA | Photosystem II | D1 protein of the PSII reaction centre |
| petB | Cytochrome b6f | Cytochrome b6 subunit; electron transfer between PSII and PSI |
| atpA | ATP synthase | α subunit of the ATP synthase; makes ATP |
| rbcL | RuBisCO | Large subunit of RuBisCO; fixes CO2 in the Calvin cycle |
| rpoB | RNA polymerase | β subunit of the plastid-encoded RNA polymerase |
| rps7 | Ribosomal protein | Small ribosomal subunit protein for translation |
| ndhF | NADH dehydrogenase | Subunit of the NDH complex; cyclic electron flow |
| matK | Maturase | Splicing of group II introns |
| clpP | Protease | Catalytic subunit of the Clp protease |

### 6. RNA and RNA-processing features
- **rRNA genes:** rrn16 (16S), rrn23 (23S), rrn4.5 (4.5S) and rrn5 (5S), present in
  both IRs (8 copies in total).
- **tRNA genes:** 37 copies (30 unique), e.g., trnH-GUG, trnK-UUU, trnM-CAU,
  trnL-UAA and trnI-GAU.
- **Genes with introns:** rps16, atpF, rpoC1, ycf3 (2 introns), clpP (2 introns),
  petB, petD, rpl16, rpl2, ndhB, rps12 and ndhA. rps12 is trans-spliced: its
  5' exon is in the LSC and its 3' exons are in the IR.
- matK encodes a maturase thought to help splice group II introns.

### 7. Pseudogenes, duplications and unusual features
- **Pseudogene:** infA (initiation factor 1) is annotated as a pseudogene.
- **Duplications:** the IR duplicates the rRNA genes, 7 tRNAs, ndhB, rpl2,
  rpl23, rps7, rps12, ycf2 and four ORFs.
- **Trans-splicing:** rps12 is split between the LSC and the IR.
- **Unassigned ORFs:** 10 hypothetical ORFs (e.g., ORF70A, ORF74, ORF99, ORF350)
  are annotated, but the RefSeq record labels them only as hypothetical proteins.
- No other gene losses or rearrangements are noted in the record.

### 8. GC content and other observations
The GC content is **37.85%** (Galaxy; 155,943 bp, 1 record, no Ns). Two other
observations:
1. GC content differs by region: LSC 35.95%, SSC 32.07% and each IR 43.22%.
   The higher IR value probably reflects the GC-rich rRNA genes (16S about
   56.6%, 23S about 55.0%).
2. The SSC carries most of the ndh genes (ndhF, ndhD, ndhG, ndhI, ndhA, ndhH) and
   ycf1, while photosystem and RNA polymerase genes lie mainly in the LSC.

### 9. Plastid vs. mitochondrial genome

**Five similarities**
1. Both descend from bacterial endosymbionts (cyanobacteria and α-proteobacteria).
2. Both are DNA genomes inside double-membrane organelles.
3. Both encode rRNAs, tRNAs and ribosomal proteins, and need nuclear-encoded proteins.
4. Both are usually maternally inherited in angiosperms.
5. Both have lost or transferred many genes to the nucleus, contain introns and
   undergo C-to-U RNA editing.

**Five differences** (see table)

| Feature | Plastid genome | Mitochondrial genome |
|---|---|---|
| Cellular location | Plastids (chloroplasts) | Mitochondria |
| Main biological functions | Photosynthesis, plastid gene expression | Respiration, ATP production |
| Typical genome organization | Single circular map with LSC, SSC and two IRs | Large, multipartite; recombining subgenomic circles and linear forms |
| Relative genome size | Small and conserved (155,943 bp here) | Larger and variable (430,597 bp in *N. tabacum*, NC_006581.1; up to Mb in plants) |
| Gene content | About 110-130 genes: photosynthesis, rRNA, tRNA, ribosomal proteins | About 50-60 genes: respiratory complexes, ribosomal proteins, few tRNAs |
| Copy number | Very high (hundreds to thousands of copies per cell) | Lower (tens to hundreds of copies) |
| Inheritance | Maternal in most angiosperms, including tobacco | Mostly maternal |
| Recombination / structural change | Conserved structure; IR-mediated recombination, rare rearrangements | Frequent recombination across repeats; rapid structural change |
| Mutation / substitution pattern | Low-to-moderate substitution rate; conserved | Very low point-mutation rate but extensive rearrangement and foreign DNA uptake |
| Common research applications | Phylogenetics, barcoding, plastid transformation, ancient DNA | Cytoplasmic male sterility, breeding, evolution of genome structure |

### 10. Practical value, limitations and research questions

**Advantages compared with the nuclear genome**
- High copy number gives high DNA yield and works with degraded or herbarium DNA.
- Small, compact and conserved, so it is easy to assemble.
- Mostly uniparental and non-recombining, which gives a clear maternal lineage
  and simple phylogenies.
- Conserved gene content allows universal primers and barcodes (rbcL, matK).
- Avoids the repeat-rich, large and sometimes poorly assembled nuclear genome
  and the problems of nuclear sex chromosomes (X/Y), which are repetitive, have
  restricted recombination and are hard to assemble.
- Useful for plastid transformation and genetic engineering.

**Limitations**
- It is effectively one locus with one (usually maternal) history, so it cannot
  show paternal contribution, hybridization or introgression.
- Low variation may not resolve closely related species.
- Plastid DNA transferred to the nucleus (NUPTs) can contaminate data.
- It carries no information on most nuclear traits, e.g., nicotine biosynthesis
  or sex determination.

**Research questions**
- *Plastid data:* Which species was the maternal parent of the allotetraploid *N. tabacum*,
  or how are *Nicotiana* species related maternally?
- *Nuclear data:* Which genes control nicotine alkaloid biosynthesis, or how did
  the two parental subgenomes evolve after hybridization?

---

## References
- NCBI RefSeq NC_001879.2, *Nicotiana tabacum* plastid, complete genome.
  https://www.ncbi.nlm.nih.gov/nuccore/NC_001879.2
- Shinozaki K, et al. (1986). The complete nucleotide sequence of the tobacco chloroplast
  genome: its gene organization and expression. *EMBO J.* 5(9):2043-2049.
- NCBI RefSeq NC_006581.1, *N. tabacum* mitochondrion, complete genome.
- usegalaxy.org (Fasta Statistics).
