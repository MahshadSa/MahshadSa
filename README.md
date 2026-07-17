# Mahshad Sarikhani

MD and research associate in abdominal radiology at Shariati Hospital, Tehran University of Medical Sciences. I work on quantitative MRI in inflammatory bowel disease, at the point where imaging methodology meets clinical decision-making.

Most of what I build starts from a problem I hit in my own research: disease activity that endoscopy measures invasively and MRE could measure better, radiology reports that hold structured information no one can query, literature that arrives faster than I can triage it. The tools here are reproducible by design, because the alternative is work that cannot be checked.

## Current focus

- Bayesian multilevel modelling for segmental Mayo Endoscopic Score triage in ulcerative colitis, using MRE features and faecal calprotectin
- Quantitative MRE in ulcerative colitis: motility, chronicity, and activity
- Working toward an agentic LLM pipeline for Lémann Index scoring from free-text MRE reports in Crohn's disease, currently at the deterministic foundation stage

## Recent

- Two first-author oral presentations at ESGAR 2026, both delivered on my behalf by Dr Gauraang Bhatnagar
- First-author motility manuscript under review at *Journal of Crohn's and Colitis*
- Ongoing collaboration with UCL and Motilent on quantitative bowel MRE

## Selected projects

**[uc-mre-activity-risk-stratifier](https://github.com/MahshadSa/uc-mre-activity-risk-stratifier)** — Bayesian ordinal regression estimating segment-level Mayo endoscopic severity from MRE features and faecal calprotectin. Marginalises the patient random intercept via Gauss-Hermite quadrature to give new-patient probabilities rather than population averages. Across 245 segments from 49 patients, marginal AUC 0.84 to 0.87; 53% of segments resolve into definitive low or high-risk tiers without endoscopy. Model constants are versioned; scope limits are explicit.
[DOI: 10.5281/zenodo.18171572](https://doi.org/10.5281/zenodo.18171572)

**[abdominal-radiology-reports](https://github.com/MahshadSa/abdominal-radiology-reports)** — Pipeline for turning free-text abdominal radiology reports into structured, queryable records, built as the data infrastructure the imaging work runs on. Patient data never enters the repository; tests use synthetic documents only. Phase 0 complete, Phase 1 in progress.

**[lemann-li-app](https://github.com/MahshadSa/lemann-li-app)** — Streamlit implementation of the updated Organ and Global Lémann Index (Pariente et al., *Gastroenterology* 2021). Research and education use only.
[DOI: 10.5281/zenodo.17513800](https://doi.org/10.5281/zenodo.17513800)

**[ibd-digest](https://github.com/MahshadSa/ibd-digest)** — A daily pipeline that fetches new IBD imaging research from PubMed and Crossref, ranks it by SPECTER2 semantic similarity against a curated corpus, and delivers a tiered digest to Obsidian. The interesting problem was calibration: SPECTER2 produces uniformly high cosine similarities on in-domain biomedical text, so fixed thresholds are useless. Tiers are anchored to corpus percentiles instead. Runs unattended on a schedule.

**[radiology-clip-mini](https://github.com/MahshadSa/radiology-clip-mini)** — A CLIP-style image-text retrieval baseline for chest radiographs and reports, built as a reference implementation others can actually run. ResNet-18 and DistilBERT encoders, symmetric InfoNCE, Grad-CAM interpretability, patient-level splits to prevent leakage. Versioned on Zenodo with CI and deterministic seeds.
[DOI: 10.5281/zenodo.17795012](https://doi.org/10.5281/zenodo.17795012)

[Google Scholar](https://scholar.google.com/citations?user=iKhNW9AAAAAJ) | [ORCID](https://orcid.org/0000-0002-0475-3064)
