# Project Oracle

## Metagenomics of agricultural soils from Burkina Faso

### Sampling and sample processing

- Sample collection (2017),
- geographical coordinates,
- DNA extraction,
- Shotgun sequencing (Illumina NovaSeq),
- 16S and ITS2 amplification and sequencing (Illumina MiSeq)

(to be written)

### From raw sequences to annotated occurrence tables

(scripts are available, will be added later)

### Statistical analysis

(see the Rmarkdown scripts, starting with
[src/04\_numerical\_ecology.Rmd](src/04_numerical_ecology.Rmd))

Note that library functions are noted as `package::function()` (for
example, `vegan::diversity()`), except for tidyverse functions and
base packages.

#### Taxonomy

temporary code to extract and prepare the Silva taxonomy:

```sh
cd ./data/Silva/

zgrep "^>" SILVA_138.1_SSURef_NR99_tax_silva.fasta.gz | \
    sed 's/^>// ; s/ /\t/1' > SILVA_138.1_SSURef_NR99_tax_silva.txt
```

**Roadmap (16S)**:

- [x] metabarcoding: decontamination and filtering,
- [x] metabarcoding: alpha diversity,
- [x] metabarcoding: alpha diversity vs locality,
- [x] metabarcoding: beta diversity vs locality,
- [x] metabarcoding: beta diversity vs locality (make a new plot with
      barycenters),
- [x] metabarcoding: use 20 taxonomic fields and weighted assignments,
- [ ] metabarcoding: taxonomy and functions (nitrogen cycle),
- [x] metagenomics shotgun: filtering,
- [ ] metagenomics shotgun: turn NMDS plot into a function,
- [ ] metagenomics shotgun: use the metabarcoding taxonomic framework,
- [ ] metagenomics shotgun: alpha diversity,
- [ ] metagenomics shotgun: alpha diversity vs locality,
- [ ] metagenomics shotgun: beta diversity vs locality,
