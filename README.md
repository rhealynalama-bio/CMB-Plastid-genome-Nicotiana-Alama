# CMB Plastid Genome: *Nicotiana tabacum*

**Student:** Rhealyn F. Alama

**Course/Section:** Cell and Molecular Biology - B

This repository documents two connected laboratory activities on the plastid
genome of *Nicotiana tabacum* (common tobacco, family Solanaceae), NCBI RefSeq
accession **NC_001879.2** (155,943 bp, circular).

## Activities

| Activity | Folder | Summary |
|---|---|---|
| 1. Characterization of a Plastid Genome | [01_Plastid_Genome_Nicotiana](01_Plastid_Genome_Nicotiana/) | Genome retrieved from NCBI, sequence statistics in Galaxy, gene content analysis, final report |
| 2. Visualize Plastid Genome Structure | [02_Plastid_Genome_Visualization](02_Plastid_Genome_Visualization/) | Circular genome map made with OGDRAW, map interpretation and answers |

## Genome at a glance
- **Size:** 155,943 bp, GC content 37.85%
- **Structure:** LSC 86,686 bp, SSC 18,571 bp, two inverted repeats of 25,343 bp each
- **Genes:** 112 unique named genes (78 protein-coding, 30 tRNA, 4 rRNA), plus one pseudogene (infA) and hypothetical ORFs

## Repository structure
```
├── 01_Plastid_Genome_Nicotiana/
│   ├── README.md
│   ├── Data/        genome FASTA and GenBank files
│   ├── Results/     Galaxy statistics and summary table
│   ├── Figures/     Galaxy screenshot
│   └── Report/      final report (Questions 1-10)
└── 02_Plastid_Genome_Visualization/
    ├── README.md
    ├── 01_Data/     original GenBank file
    ├── 02_Figures/  OGDRAW genome map
    └── 03_Answers/  answers to the visualization questions
```

## Key files
- [Activity 1 README](01_Plastid_Genome_Nicotiana/README.md)
- [Final report](01_Plastid_Genome_Nicotiana/Report/Plastid_Genome_Report_Nicotiana_tabacum.md)
- [Summary table](01_Plastid_Genome_Nicotiana/Results/plastome_summary_table.md)
- [Activity 2 README](02_Plastid_Genome_Visualization/README.md)
- [Answers](02_Plastid_Genome_Visualization/03_Answers/Lab_plastid_genome_answers.md)

## Tools
NCBI Nucleotide (RefSeq), usegalaxy.org (Fasta Statistics), OGDRAW v1.3.1, GitHub.

## References
- NCBI RefSeq NC_001879.2, *Nicotiana tabacum* plastid, complete genome. https://www.ncbi.nlm.nih.gov/nuccore/NC_001879.2
- Shinozaki K, et al. (1986). The complete nucleotide sequence of the tobacco chloroplast genome. *EMBO J.* 5(9):2043-2049.
- Greiner S, Lehwark P, Bock R. (2019). OrganellarGenomeDRAW (OGDRAW) version 1.3.1. *Nucleic Acids Research* 47:W59-W64.
