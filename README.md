# Genotypic AMR Prediction in *Klebsiella pneumoniae*

## Project Overview

This project performs a genotypic antimicrobial resistance (AMR) analysis of *Klebsiella pneumoniae* NTUH-K2044 using genome sequence data and AMRFinderPlus.

The analysis focuses on identifying antimicrobial resistance determinants, virulence-associated features, stress/metal-resistance features, genomic locations, and mutation-specific records.

## Objectives

- Identify antimicrobial resistance (AMR) determinants.
- Classify detected AMR determinants.
- Determine the genomic location of detected determinants.
- Identify virulence-associated features.
- Identify stress/metal-resistance features.
- Perform an organism-specific mutation search.
- Generate structured result tables and visual summaries.
- Interpret genotypic AMR findings while distinguishing genotype from phenotype.

## Organism

*Klebsiella pneumoniae* NTUH-K2044

## Input Genome

The analysis used a FASTA genome file containing chromosome and plasmid sequences of *Klebsiella pneumoniae* NTUH-K2044.

## Software

- AMRFinderPlus 4.2.7
- AMRFinderPlus Database 2026-08-07.1

## Analysis Workflow

1. Input genome quality and FASTA-header check
2. AMRFinderPlus installation and database setup
3. Genome-wide AMR and resistance-feature detection
4. Classification of detected determinants
5. Genomic-location analysis
6. Organism-specific mutation search
7. AMR evidence table generation
8. Statistical summaries and visualization
9. Final interpretation

## Results

### Genotypic AMR Analysis

Six AMR determinants were identified:

- **fosA**: fosfomycin resistance-associated determinant
- **kdeA**: multidrug efflux-associated determinant
- **blaSHV-11**: class A beta-lactamase
- **oqxA**: multidrug efflux-associated determinant
- **oqxB19**: phenicol/quinolone-associated efflux determinant
- **emrD**: multidrug efflux-associated determinant

All six AMR determinants were located on chromosome **NC_012731.1**.

### Virulence-associated Features

The analysis identified **21 virulence-associated features**, including features associated with:

- Mucoid phenotype regulation
- Salmochelin
- Aerobactin
- Yersiniabactin

Several of these features were located on plasmid **NC_006625.1**.

### Stress and Metal Resistance

A total of **19 stress/metal-associated features** were detected, including systems associated with:

- Copper
- Silver
- Tellurium
- Other metal-associated stress responses

Most of these features were located on plasmid **NC_006625.1**.

### Mutation Analysis

An organism-specific AMRFinderPlus analysis was performed for *Klebsiella pneumoniae*. No mutation-specific records were detected in the resulting AMRFinderPlus output.

## Overall Summary

| Feature | Number |
|---|---:|
| AMR determinants | 6 |
| Virulence-associated features | 21 |
| Stress/metal resistance features | 19 |
| Mutation-specific records | 0 |

## Interpretation

The analysis identified multiple AMR determinants together with virulence-associated and stress/metal-resistance features. The detected AMR determinants were located on the chromosome, while several virulence-associated and stress/metal-resistance features were detected on the plasmid.

Genotypic detection of AMR determinants does not by itself confirm the actual antimicrobial susceptibility phenotype. Phenotypic antimicrobial susceptibility testing would therefore be required for experimental validation.

## Output Files

The analysis generated the following structured result files:

- `results/AMR_evidence_table.csv`
- `results/Virulence_factors.csv`
- `results/Stress_metal_resistance.csv`
- `results/AMR_mutation_results.csv`
- `results/Project_summary.csv`

## Repository Contents

- `Genotypic_AMR_Prediction_Pipeline.ipynb` - complete analysis workflow
- `results/` - structured analysis results
- `README.md` - project documentation

## Limitations

This project represents a **genotypic prediction** of antimicrobial resistance. The presence of a resistance determinant does not necessarily establish phenotypic antimicrobial resistance. Experimental antimicrobial susceptibility testing would be required for confirmation.
