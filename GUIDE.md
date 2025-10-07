# SAP Folder Structure Guide

This guide explains how to use the clean folder structure for Statistical Analysis Plan (SAP) work.

## Folder Overview

### 1. data/
Store all your data files here:
- **raw/**: Keep your original, unmodified data files here. Never edit these files directly.
- **processed/**: Store cleaned, processed, and analysis-ready datasets here.

### 2. analysis/
All your analysis code goes here:
- **scripts/**: R, Python, SAS, or other analysis scripts
- **models/**: Statistical models, model objects, and model outputs

### 3. documentation/
Project documentation and reports:
- **sap/**: Statistical Analysis Plan documents and related materials
- **reports/**: Analysis reports, study summaries, and documentation

### 4. output/
Generated outputs from your analyses:
- **figures/**: All plots, graphs, and visual outputs
- **tables/**: Tables, summary statistics, and tabular results

## Best Practices

1. **Keep raw data intact**: Never modify files in `data/raw/`
2. **Document your work**: Add README files in subdirectories as needed
3. **Version control**: The `.gitignore` file keeps large data and output files out of git while preserving the folder structure
4. **Organize by project**: Consider creating subdirectories within these folders for different studies or analyses

## Getting Started

1. Place your raw data in `data/raw/`
2. Create your data cleaning scripts in `analysis/scripts/`
3. Save processed data to `data/processed/`
4. Write your SAP in `documentation/sap/`
5. Run analyses and save outputs to `output/`

## Note on .gitignore

The `.gitignore` file is configured to:
- Keep the folder structure in version control (via `.gitkeep` files)
- Exclude large data files and generated outputs
- Ignore temporary and system files

This ensures the repository stays clean while maintaining the organizational structure.
