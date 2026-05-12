# scRNA-seq Cell Type Classifier

## Biological question

Can we classify immune cell types from scRNA-seq count matrices
using classical ML (XGBoost) and a shallow MLP?

## Data

* PBMC 3k dataset (10x Genomics)
* 2,700 peripheral blood mononuclear cells

## Methods

* Preprocessing: scanpy QC, normalization, HVG selection
* Models: XGBoost, MLP (PyTorch)
* Evaluation: 5-fold CV, F1, confusion matrix, UMAP

## Results

| Model   | Accuracy | Weighted F1 |

|---------|----------|-------------|

| XGBoost | *0.992*    | *0.992*       |

| MLP     | *0.996*    | *0.996*       |

&#x20;



Setup

```bash
conda env create -f environment.yml
conda activate genomics-ml
```

