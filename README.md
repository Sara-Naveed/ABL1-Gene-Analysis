# ABL1 Gene Analysis

## Overview
This project analyzes the ABL1 gene which produces Tyrosine-protein kinase ABL1.
ABL1 is an oncogene whose fusion with BCR gene causes Chronic Myeloid Leukemia (CML).
Imatinib (Gleevec) is used as a drug to treat CML by binding to ABL1 kinase domain.

---

## Step 1 - DNA Sequence
- Gene: ABL1 (Homo sapiens)
- NCBI Accession: NM_005157.6
- Source: NCBI Nucleotide Database

[>ABL1 DNA Sequence (NM_005157.6)
GTTAACAGGCGCGTCCCGGCCAGGCGGAGACGCGGCCGCGGCCATGGGCGGGCGCGGGCGCGCGGGGCGG
CGGTGAGGGCGGCTGGCGGGGCCGGGGGCGCCGGGGGGGCGCGCGGGCCGAGCCGGGCCTGAGCCGGGCC
CGCGGACCGAGCTGGGAGAGGGGTTCCGGCCCCCGACGTGCTGGCGCGGGAAAATGTTGGAGATCTGCCT
GAAGCTGGTGGGCTGCAAATCCAAGAAGGGGCTGTCCTCGTCCTCCAGCTGTTATCTGGAAGAAGCCCTT]

---

## Step 2 - DNA to mRNA Conversion
- Converted DNA sequence to mRNA by replacing Thymine (T) with Uracil (U)
- Done using Python string replacement

---

## Step 3 - BLAST Results
- Tool: NCBI BLAST (blastn)
- Top Hit: ABL1, Homo sapiens
- Identity: 100%
- E-value: 0.0

---

## Step 4 - Protein Sequence
- Protein: Tyrosine-protein kinase ABL1
- UniProt: P00519
- Length: 1130 amino acids

---

## Step 5 - AlphaFold2 Structure
- Downloaded from AlphaFold EBI Database
- Accession: AF-P00519-F1-v6
- Average pLDDT: 63.38

<img width="2100" height="600" alt="ABL1_pLDDT_plot" src="https://github.com/user-attachments/assets/9f548890-193c-4656-b18d-d277cfb9efb3" />


---

## Step 6 - Structure Verification
- Compared AlphaFold structure with Crystal structure (PDB: 1IEP)
- RMSD: 5.022 Å (Kinase domain)
- Moderate deviation expected due to full protein vs domain comparison

---

## Step 7 - GNINA Ligand Docking
- Receptor: ABL1 kinase (1IEP.pdb)
- Ligand: Imatinib (Gleevec) - PubChem CID 5291
- Tool: GNINA molecular docking
- Best Affinity Score: -9.50 kcal/mol (Mode 9)
- Strong binding confirmed

### Docking Results Table
| Mode | Affinity (kcal/mol) |
|------|-------------------|
| 1 | -6.83 |
| 5 | -7.82 |
| 6 | -9.39 |
| 9 | -9.50 |

<img width="1123" height="702" alt="ABL1_pLDDT_plot png1" src="https://github.com/user-attachments/assets/e5cb3414-8c32-471e-9694-0fc1a91c3a74" />


---

## Tools Used
- NCBI Nucleotide & Protein Database
- Biopython
- NCBI BLAST
- AlphaFold EBI Database
- GNINA Molecular Docking
- Mol* Viewer>

