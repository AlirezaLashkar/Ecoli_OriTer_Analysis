# Ori/Ter Detection in Escherichia coli K-12 MG1655

**Author:** Alireza Lashkarbolooki  
**Degree:** M.Sc. Bioinformatics, Sharif University of Technology  
**Course:** Introduction to Bioinformatics, Dr. Ali Sharifi Zarchi  
**Date:** October 20, 2025

---

## Project Overview

This project detects the **origin of replication (Ori)** and **terminus (Ter)** in the *Escherichia coli* K-12 MG1655 genome.  
Accurate identification of Ori and Ter is crucial for understanding genome replication, replication timing, and nucleotide composition patterns.

We use multiple computational indicators to predict Ori/Ter positions and compare them with reference annotations from **NCBI** and **EcoCyc**.

**Genome reference:**  
- [NC_000913.3 - E. coli K-12 MG1655, complete genome](https://www.ncbi.nlm.nih.gov/nuccore/556503834)  
- [oriC site in EcoCyc](https://ecocyc.org/ECOLI/NEW-IMAGE?type=EXTRAGENIC-SITE&object=G0-10506)

---

## Indicators Used

1. **GC Skew**  
   Measures the imbalance between guanine (G) and cytosine (C) nucleotides in a sliding window along the genome. Shifts in GC skew often indicate Ori/Ter regions.

2. **Cumulative GC Skew**  
   Tracks the running sum of GC skew to highlight large-scale nucleotide composition shifts.

3. **AT Skew**  
   Measures the imbalance between adenine (A) and thymine (T) nucleotides. Similar to GC skew, AT skew can indicate replication origins or termini.

4. **Cumulative AT Skew**  
   Running sum of AT skew to detect global trends along the genome.

5. **G and C Densities**  
   Fraction of guanine and cytosine nucleotides in each window. Local density variations often correlate with replication-related features.

6. **G/C Ratio**  
   Compares the relative abundance of G to C nucleotides. Helps detect local nucleotide composition biases.

7. **GC/AT Ratio**  
   Compares the combined abundance of G and C to that of A and T nucleotides. Useful for identifying replication-associated asymmetries.

---

## Installation

1. Clone repository:

```bash
git clone https://github.com/AlirezaLashkar/Ecoli_OriTer_Analysis.git
cd Ecoli_OriTer_Analysis

