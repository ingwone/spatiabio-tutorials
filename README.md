# SpatiaBio Tutorials

Code and notebooks from [spatiabio.com](https://www.spatiabio.com) — a blog covering spatial transcriptomics and single-cell genomics. Every analysis here is run on real data with verified outputs.

## Posts & Notebooks

| # | Post | Notebook |
|---|------|----------|
| 1 | [Squidpy vs Seurat: A Practical Comparison](https://www.spatiabio.com/2026/06/squidpy-vs-seurat-for-spatial.html) | [squidpy-vs-seurat/squidpy_vs_seurat.ipynb](squidpy-vs-seurat/squidpy_vs_seurat.ipynb) |
| 2 | [Squidpy + Seurat Troubleshooting Roundup](https://www.spatiabio.com/2026/06/squidpy-seurat-spatial-transcriptomics.html) | [troubleshooting/squidpy_seurat_troubleshooting.ipynb](troubleshooting/squidpy_seurat_troubleshooting.ipynb) |
| 3 | [Spatio-DARLIN: The Paper That Maps Where Cells Have Been](https://www.spatiabio.com/2026/06/spatio-darlin-paper-that-maps-where.html) | [spatio-darlin/spatio_darlin_explainer.ipynb](spatio-darlin/spatio_darlin_explainer.ipynb) |
| 4 | [CellChat on Spatial Data: A Step-by-Step Tutorial](https://www.spatiabio.com/2026/06/cellchat-on-spatial-data-step-by-step.html) | [cellchat-spatial/cellchat_spatial_tutorial.ipynb](cellchat-spatial/cellchat_spatial_tutorial.ipynb) |
| 5 | [Spatially Variable Genes with Squidpy: Moran's I](https://www.spatiabio.com/2026/06/spatially-variable-genes-with-squidpy.html) | [svg-morans-i/svg_morans_i.ipynb](svg-morans-i/svg_morans_i.ipynb) |
| 6 | [Visualizing Spatially Variable Genes with Squidpy](https://www.spatiabio.com/2026/06/visualizing-spatially-variable-genes-on.html) | [svg-visualization/svg_visualization.ipynb](svg-visualization/svg_visualization.ipynb) |
| 7 | [Neighborhood Enrichment Analysis with Squidpy](https://www.spatiabio.com/2026/07/neighborhood-enrichment-analysis-with.html) | [nhood-enrichment/nhood_enrichment.ipynb](nhood-enrichment/nhood_enrichment.ipynb) |
| 8 | [Co-occurrence Analysis with Squidpy](https://www.spatiabio.com/2026/07/co-occurrence-analysis-with-squidpy.html) | [co-occurrence/co_occurrence.ipynb](co-occurrence/co_occurrence.ipynb) |
| 9 | [Ligand-Receptor Interactions with Squidpy](https://www.spatiabio.com/2026/07/ligand-receptor-interactions-in-spatial.html) | [ligrec/ligrec.ipynb](ligrec/ligrec.ipynb) |
| 10 | [Complete Squidpy Spatial Transcriptomics Workflow](https://www.spatiabio.com/2026/07/complete-squidpy-spatial.html) | [complete-workflow/complete_workflow.ipynb](complete-workflow/complete_workflow.ipynb) |
| 21 | [I Gave Claude Science One Prompt. It Ran a Full Spatial Analysis.](https://www.spatiabio.com/2026/07/i-gave-claude-science-one-prompt-it-ran.html) | — |

## Pack 1 — Squidpy Foundations (16 notebooks, $19)

Available at [lociven.gumroad.com/l/squidpy-pack](https://lociven.gumroad.com/l/squidpy-pack)

| # | Notebook | Topic |
|---|----------|-------|
| 00 | `00_environment_setup.ipynb` | Conda setup, package versions, Space Ranger structure |
| 01 | `01_setup_data_loading.ipynb` | Loading AnnData, QC metrics, coordinate validation |
| 02 | `02_clustering.ipynb` | Normalization, PCA, Leiden clustering, marker genes |
| 03 | `03_spatial_neighbors.ipynb` | Delaunay vs kNN vs radius graphs, coord_type selection |
| 03b | `03b_large_dataset_memory.ipynb` | Chunked processing, sparse matrices, memory optimization |
| 04 | `04_neighborhood_enrichment.ipynb` | nhood_enrichment, z-score interpretation, n_perms guide |
| 05 | `05_co_occurrence.ipynb` | Co-occurrence vs distance, peak analysis, decay curves |
| 06 | `06_spatial_autocorrelation.ipynb` | Moran's I, spatially variable genes, Geary's C |
| 06b | `06b_batch_correction_spatial.ipynb` | Harmony, BBKNN, cross-sample nhood_enrichment |
| 07 | `07_ligrec.ipynb` | Ligand-receptor analysis, CellPhoneDB, spatial filtering |
| 08 | `08_svg_visualization.ipynb` | Custom colormaps, multi-panel figures, publication formatting |
| 09 | `09_squidpy_vs_seurat.ipynb` | Side-by-side comparison, benchmark timings |
| 10 | `10_complete_workflow.ipynb` | End-to-end pipeline in one notebook |
| 11 | `11_result_interpretation.ipynb` | Biological interpretation guide, methods text template |
| 12 | `12_common_errors_debug.ipynb` | Error diagnosis and fixes for all common failures |
| 13 | `13_publication_figures.ipynb` | Nature-style 3-panel figures, DPI/font/colormap standards |

## Data

Tutorials use publicly available datasets:
- `visium_hne_adata` — 10x Genomics Visium mouse brain (built into squidpy)
- `stxBrain` — 10x Genomics Visium mouse brain anterior (SeuratData)
- `sc_mouse_cortex` — Allen Brain Atlas scRNA-seq mouse cortex

## Environment

```bash
pip install squidpy scanpy
```

R tutorials require: `Seurat`, `SeuratData`, `CellChat`

## About

Posts are written by Lociven. All code is executed before publication.  
Full writeups at [spatiabio.com](https://www.spatiabio.com).
