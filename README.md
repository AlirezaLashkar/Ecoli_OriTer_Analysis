# Ori/Ter Detection in Escherichia coli K-12 MG1655

**Author:** Alireza Lashkarblouki  
**Degree:** M.Sc. Bioinformatics, Sharif University of Technology  
**Course:** Introduction to Bioinformatics, Dr. Ali Sharifi Zarchi  
**Date:** October 20, 2025

---

## Project Overview

This repository contains a comprehensive bioinformatics project aimed at detecting **replication origin (Ori)** and **terminus (Ter)** positions in the *Escherichia coli* K-12 MG1655 genome. Accurate identification of Ori and Ter is essential for understanding genome replication, replication timing, and nucleotide composition biases.

The project leverages multiple computational indicators:

- GC skew and cumulative GC skew
- AT skew and cumulative AT skew
- G and C nucleotide densities
- Nucleotide ratios: G/C and (G+C)/(A+T)

Predicted positions are compared against reference genome annotations from **NCBI** and **EcoCyc**.

**Genome reference:**  
[NC_000913.3 - E. coli K-12 MG1655, complete genome](https://www.ncbi.nlm.nih.gov/nuccore/556503834)  
[oriC site in EcoCyc](https://ecocyc.org/ECOLI/NEW-IMAGE?type=EXTRAGENIC-SITE&object=G0-10506)

---

## Features

1. **Sliding Window Analysis:** Computes GC/AT skew, densities, and ratios over defined windows along the genome.  
2. **Cumulative Metrics:** Tracks cumulative GC and AT skew to identify shifts in nucleotide composition.  
3. **Visualization:** Generates plots for all indicators with predicted Ori and Ter marked.  
4. **Reference Comparison:** Calculates circular distances between predicted and reference positions and assesses reliability.  
5. **Educational:** Includes formulas and detailed explanations for each metric.

---

## Methodology

### 1. GC and AT Skews
GC Skew = (G - C) / (G + C)

- **GC skew:**  
