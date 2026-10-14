# Lysosomal Enzyme Analysis — CTSH

**Enzyme:** Cathepsin H (pro-cathepsin H isoform a preproprotein)

**Gene Symbol:** CTSH

**NCBI Protein Accession:** [NP_004381.2](https://www.ncbi.nlm.nih.gov/protein/NP_004381.2)

**Accession Type:** Full‑length human RefSeq protein (MANE Select)

---

## Enzyme Function
CTSH (Cathepsin H) is a lysosomal cysteine protease of the papain family. It acts as both an **endopeptidase** (cleaves within protein chains) and an **aminopeptidase** (removes amino acids from the N‑terminus). It degrades proteins and peptides inside the lysosome, recycles amino acids, processes antigens for immune presentation, matures prohormones and proenzymes, and supports normal tissue remodeling.

---

## Results & Figures

### Figure 1 — Amino Acid Composition
![Amino Acid Composition](figures/CTSH_amino_acid_composition.png)

### Figure 2 — Potential N‑Glycosylation Motif Positions
![N-Glycosylation Motifs](figures/CTSH_potential_N_glycosylation.png)

---

## Answers to Lab Questions

### 1. What does your enzyme normally break down inside lysosomes?
CTSH degrades a broad range of substrates including general intracellular proteins, extracellular matrix components such as collagen and elastin, peptide hormones, and lysosomal proenzymes. It breaks these into smaller peptides and free amino acids that are recycled back into the cell’s amino acid pool.

### 2. What is the total length of your protein, and which amino acids are most common?
- **Total length:** 335 amino acids
- **Most common residues:**
  1. Alanine (A) — 29 counts (8.66%)
  2. Glycine (G) — 29 counts (8.66%)
  3. Lysine (K) — 23 counts (6.87%)
  4. Serine (S) — 23 counts (6.87%)
  5. Leucine (L) — 22 counts (6.57%)
- Full table: `results/CTSH_amino_acid_counts.csv`

### 3. How many potential N‑glycosylation motifs did you find? Where are they located?
- **Motif definition:** N‑X‑S/T, where X ≠ Proline
- **Total found:** 3 potential N‑glycosylation sites
- **Positions & sequences:**
  - Position 72 → N‑H‑T
  - Position 101 → N‑C‑S
  - Position 230 → N‑I‑T
- Full table: `results/CTSH_motif_positions.csv`

### 4. Why can glycosylation matter for lysosomal proteins? Does finding a motif prove the protein is glycosylated?
- **Biological importance:** N‑glycosylation aids proper protein folding, stability, and solubility in the acidic lysosomal environment. Many lysosomal proteins receive **mannose‑6‑phosphate (M6P)** tags on their glycans, these tags are recognized by receptors in the Golgi and deliver the protein specifically to lysosomes. Without correct glycosylation, the protein may misfold, be secreted instead of targeted, or be degraded prematurely.
- **Does finding a motif prove glycosylation? NO.** N‑X‑S/T is only a *sequence consensus pattern*. Actual glycosylation requires correct protein folding, enzyme accessibility, and appropriate cellular conditions. Sequence analysis alone cannot confirm that modification occurred.

### 5. What could happen in the cell if your enzyme did not work properly?
Loss or reduced CTSH activity leads to:
- Impaired lysosomal protein degradation → accumulation of undigested material → lysosomal storage‑like pathology
- Defective antigen processing → weakened immune presentation
- Abnormal tissue remodeling → connective tissue and bone homeostasis defects
- Disrupted proenzyme/prohormone maturation → broader metabolic imbalance
- In severe cases: cellular inflammation, tissue damage, and disease progression

---

## References

- **NCBI Protein:** Cathepsin H — NP_004381.2. National Center for Biotechnology Information (2026).  
  https://www.ncbi.nlm.nih.gov/protein/NP_004381.2 — Accessed 14 Oct 2026
- **UniProt:** P09668 (CTSH). UniProt Consortium — https://www.uniprot.org/uniprotkb/P09668
- **R & Packages:** R Core Team (2024); `rentrez` (v1.2.3); `ggplot2` (Wickham, 2016)
- **Function:** CTSH = lysosomal cysteine protease — endopeptidase + aminopeptidase activity; protein turnover, immune processing, tissue remodeling

  ## Github URL:** https://github.com/Jayeydd/lysosomal-enzyme-CTSH
