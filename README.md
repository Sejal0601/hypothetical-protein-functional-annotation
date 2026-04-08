🧬 Functional Annotation of Hypothetical Proteins

This project focuses on assigning biological functions to hypothetical proteins using a combination of sequence similarity, structural analysis, and evolutionary conservation.

🔍 Background

A large fraction of proteins in organisms like E. coli and Mycobacterium tuberculosis remain annotated as hypothetical proteins. These proteins lack experimentally validated functions despite being encoded in the genome.

Understanding their function is critical for:

Identifying novel drug targets
Understanding metabolic pathways
Advancing systems biology
⚙️ Methodology

This pipeline integrates multiple computational approaches:

1. Sequence Similarity Search
BLASTp against NR and PDB databases
Filtering hits based on identity (40–90%) and coverage
2. Structural Analysis
Use of AlphaFold-predicted structures
Structural alignment with known proteins
3. Multiple Sequence Alignment (MSA)
Identification of conserved residues
Functional motif detection
4. Functional Inference
Mapping conserved regions
Comparing with known protein domains
🔬 Workflow
Input sequence → BLAST → Filter hits → Retrieve sequences →
MSA → Identify conserved regions → Structural comparison →
Functional annotation

🚀 Features
  Automated BLAST pipeline
  Sequence filtering based on identity thresholds
  Integration with structural data
  Scalable for large datasets

🧪 Dataset
  Organisms: E. coli, Mycobacterium tuberculosis H37Rv
  Source: NCBI RefSeq
  
🛠 Requirements
  python 3.8+
  biopython
  pandas
  blast+
  
▶️ Usage
python scripts/run_blast.py input.fasta

📌 Author
Sejal Agarwal
Bioinformatics | Structural Biology | Computational Biology
