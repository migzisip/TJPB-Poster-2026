# TJPB-Poster-2026
Detailed information about my poster for Japan-Taiwan Plant Biology 2026 (Tokyo)

# Poster no. __: AI-based large-scale structural modeling integrated with multi-omics reveals candidate plant receptor–peptide interactions from *Pseudomonadales* microbiota

## Poster walkthrough

### Big picture

- Plant-associated microbiota influence host immunity via microbial molecules, including peptides released/secreted during cell turnover.
- Plants perceive these cues through pattern-recognition receptors (PRRs), but the broader landscape of PRR–peptide specificity across microbiota remains largely unexplored.
- This work presents a scalable framework integrating peptidomics + transcriptomics + AlphaFold3 structural modeling to prioritize candidate PRR–peptide interactions from an order-specific microbiota community. 

### Section 1: Core – Microbiota

- Inoculation with order-specific commensal bacteria in Arabidopsis induces an order-specific transcriptional signature.
- Transcriptome analysis highlights differential regulation of PRRs, supporting the idea that PRRs may contribute to perceiving order-specific microbial patterns.

### Section 2: Peptide landscape detected from Pseudomonadales order-specific SynCom

- As a proof-of-concept, the analysis focuses on order Pseudomonadales (SynCom4; 4 strains), selected because it triggers many plant PRRs.
- Proteomics and peptidomics identify >300 naturally occurring peptide fragments derived from diverse precursor proteins. 
- Example precursor categories include motility-related proteins (e.g., flagellin), cell envelope–associated proteins (e.g., OmpA family, Pal), type VI secretion components (e.g., Hcp), and cold-shock proteins.
- Signal peptide analysis (SignalP) indicates that a substantial fraction of precursors (~50%) contain secretion signals, consistent with the idea that some peptides may originate from periplasmic or extracellular

### Section 3: Large-scale AI-based structure-guided prediction of receptor–peptide interactions

- Peptide sequences detected in Pseudomonadales peptidomics are paired with PRR ectodomains selected from receptors that are constitutively expressed or upregulated during microbiota association.
- Using AlphaFold3, the workflow models ~13,000 pairwise receptor–peptide complexes to generate an interaction landscape that can be filtered to prioritize testable hypotheses. 

### Section 4: Structural modeling reveals widespread binding potential of plant PRRs to Pseudomonadales peptides

- Candidate interactions are prioritized using interface predicted TM (iPTM) as a confidence metric for binding likelihood.
- With a stringent iPTM > 0.8 threshold, the workflow yields 151 high-confidence PRR–peptide pairs, originating from 67 precursor proteins (36/67 precursors contain signal peptides).
- High-confidence candidates span multiple PRR families (LecRK, MALK, LRR-RLK, LRR-RLP, LYM), suggesting broad potential for PRR engagement by microbiota-derived peptides.

### Section 5: High‑iPTM PRR–peptide pair map to BAK1 co‑receptor architecture

- High-confidence PRR–peptide candidates are mapped onto known cell-surface co-receptor modules, including BAK1 and SOBIR1, linking predicted binding events to established immune signaling architectures. 
- A known reference complex (FLS2 ectodomain + flg22 + BAK1 ectodomain) is shown as a benchmark for PRR–ligand complex modeling, providing a familiar point of comparison for predicted interaction confidence.
- We identified one candidate involving an LRR-RLK (7110) and a peptide derived from type VI secretion system tube protein Hcp, with a modeled association to BAK1 ectodomain at high confidence.

### Section 6:  SynCom4 heat-killed cells (HK) and cell-free supernatant (CFS) elicit distinct immune outputs across bioluminescent reporter lines

To assess whether SynCom4-derived material activates plant immune signaling, immune outputs were monitored using LUMI-map reporter lines, which express the luciferase (LUC) gene fused to promoters of defense-related genes. These promoters are associated with downstream immune signaling and pattern-triggered immunity (PTI), enabling real-time quantification of transcriptional activation.

Bioluminescence reporter assays show immune outputs after treatment with:

- flg22 (positive control),
- heat-killed SynCom4 (HK),
- cell-free supernatant (CFS),
- water (negative control).

Multiple immune reporters (e.g., WRKY and other defense-associated promoters) display distinct temporal response patterns, consistent with SynCom-derived material containing immune-active cues.

### Section 7: Summary and future work

- The framework links multi-omics discovery to structure-guided prioritization of candidate PRR–peptide interactions from microbiota.
- Future work focuses on validation, including combinatorial gRNA editing of PRRs in reporter backgrounds and testing prioritized microbiota peptides. 

---


![Preview](docs/JTPB_2026_Poster_1st_draft_v3.jpg)

[Download / Open full PDF](docs/TJTPB_2026_Poster_1st_draft_v3.pdf)


