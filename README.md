# From Raw Biological Data to Structured Information
### A Bioinformatics Workshop — Data in Biology Day

---

**Presenter:** Souhil MOKEDDEM  
**Event:** Data in Biology Day  
**Organized by:** Data Science Club USTHB  ×  Quanta Club  
**Contact:** mokeddemsouhil968@gmail.com · [LinkedIn](https://linkedin.com/in/souhil-mokeddem-aa979435b)

---

## What This Repository Contains

| File | Description |
|------|-------------|
| `bioinformatics_workshop.pptx`[bioinformatics_workshop.pptx] | Full 20-slide presentation deck |
| `bioinformatics_workshop_demo.ipynb`[bioinformatics_workshop_demo.ipynb] | Live Python demo notebook |

---

## The Presentation — `bioinformatics_workshop.pptx`

A complete 20-slide workshop deck designed for a mixed audience of biology students, medical students, and data science beginners.

**Covers:**
- History of DNA sequencing — from Sanger (1977) and the Human Genome Project to modern NGS and 3rd generation platforms
- Types of biological data and common raw file formats (FASTA, FASTQ, BAM, count matrices)
- The FASTA and FASTQ formats in detail — what headers contain, how quality scores are encoded (ASCII/Phred)
- Why raw data cannot be used directly — 6 failure modes, each with a concrete example
- Quality Control (QC) — what metrics matter and how FastQC works
- Filtering and trimming — the logic behind each threshold
- Transformation — from text sequences to structured numeric datasets
- The complete preprocessing pipeline end-to-end
- Real biomedical applications — cancer genomics, Alzheimer's research, COVID-19 tracking, rare disease diagnosis, drug response prediction — with data quality impact tables
- Live demo walkthrough slide

**Audience:** No prior bioinformatics or data science knowledge required.  
**Image placeholders** are included throughout — search keywords are embedded directly in each placeholder for easy replacement.

---

## The Demo Notebook — `bioinformatics_workshop_demo.ipynb`

A fully self-contained Python demo that simulates a realistic bioinformatics preprocessing pipeline from scratch.

**Requirements:** Python 3 · pandas · no specialized libraries

**What the notebook does, step by step:**

1. Simulates 30 raw sequencing reads with realistic quality variation (good reads, low-quality reads, short reads, N-heavy reads)
2. Calculates QC metrics per read — average Phred quality score, read length, N-fraction, GC content
3. Prints a QC report showing data quality before any filtering
4. Applies three filters — quality threshold, length threshold, N-fraction threshold — and logs the reason each read is removed
5. Transforms clean sequences into a numeric feature table (base composition per read)
6. Aggregates results to a per-sample summary table ready for downstream analysis

**Why it matters:** Every step mirrors what production bioinformatics tools do (FastQC, Trim Galore, Fastp) — just in plain Python so the logic is fully visible.

---


*Presented at Data in Biology Day — a collaboration between Data Science Club USTHB and Quanta Club.*
