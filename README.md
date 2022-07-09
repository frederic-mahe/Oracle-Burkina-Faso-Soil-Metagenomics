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

**Roadmap (16S)**:

- [x] metabarcoding: decontamination and filtering,
- [x] metabarcoding: alpha diversity,
- [x] metabarcoding: alpha diversity vs locality,
- [x] metabarcoding: beta diversity vs locality,
- [ ] metabarcoding: beta diversity vs locality (make a new plot with
      barycenters),
- [ ] metabarcoding: use 20 taxonomic fields and weighted assignments,
- [ ] metabarcoding: taxonomy and functions (nitrogen cycle),
- [ ] metagenomics shotgun: use the metabarcoding taxonomic framework,
- [ ] metagenomics shotgun: same stats as above,
