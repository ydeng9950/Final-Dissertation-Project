# Final-Dissertation-Project
Final Dissertation Project

# Purpose

This notebook contains the full set of experiments for the dissertation Probing Discourse Structure in Dialogue: Evaluating and Fine-Tuning RoBERTa and BART on Sentence Ordering and Next Sentence Prediction. It brings together the preprocessing, training, and evaluation steps for two transformer models (BART and RoBERTa) tested on dialogue data from the STAC corpus. The aim is to see how far these models can handle discourse coherence when probed with sentence ordering and next sentence prediction (NSP) tasks.

# Contents

The notebook is organised in sections that reflect the workflow of the project:

Corpus upload – loading the STAC data used in all experiments.

BART sentence ordering – data preparation, fine-tuning, evaluation, and a baseline run with the pre-trained model.

RoBERTa sentence ordering – setting up the reranker, training, and evaluation.

NSP experiments – binary classification of EDU adjacency for both models.

Significance testing and exports – utilities for statistical comparisons and saving results (CSV files) used in the dissertation write-up.

# Dependencies

The notebook was written for Python and relies on widely used libraries:

torch and transformers for model training

numpy, pandas, scipy, sklearn for data handling and evaluation

tqdm for progress bars

matplotlib for visualisation

The experiments were run on GPU (Google Colab), but they can be reproduced in any environment with sufficient memory and compute.

# How to Use

Upload the STAC dataset into your environment.

Run the cells in order, starting with the corpus upload.

Training checkpoints and evaluation outputs are written to the working directory.

Exported CSV files provide the per-dialogue and relation-level scores reported in the dissertation.

# Notes

All paths, filenames, and metadata have been cleaned so the notebook can be shared without identifiers.

This file is intended as an appendix to the dissertation and as a record of the methods used.

To reproduce results, the same model checkpoints (facebook/bart-base and roberta-base) and the same version of the STAC corpus should be used.
