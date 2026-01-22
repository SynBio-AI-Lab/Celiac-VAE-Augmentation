# Raw Data (Not Included)

This repository does **not** distribute raw patient-level data.

To ensure full reproducibility while respecting data governance and licensing constraints, users are instructed to manually download the original dataset from a public source.

## Dataset Source
- **NCBI Gene Expression Omnibus (GEO)**
- **Accession ID:** GSE134900
- **Disease:** Celiac disease
- **Data Type:** Normalized gene expression matrix (human)

## Download Instructions
1. Visit the following URL:
   https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE134900
2. Download the normalized expression file:
   `GSE134900_normalized_expr.valerie_celiac.human.csv.gz`
3. Place the downloaded file into this directory:
   `data/raw/`

## Reproducibility Note
All preprocessing, normalization, and filtering steps used in the paper are fully automated and implemented in the provided scripts (e.g., `generate_synthetic_data.py`).  
No manual preprocessing is required beyond downloading the dataset.

This design ensures that all experimental results reported in the paper can be independently reproduced starting from the same public raw data source.

