# GEO-Aligned

## Introduction
GEO-Aligned is a semantic parsing dataset that was obtained by augmenting the popular GeoQuery data with word alignment information. 

It comes in three languages:
- 🇺🇸 English, based on the [original dataset](https://dl.acm.org/doi/10.5555/1864519.1864543)
- 🇩🇪 German, based on [multilingual GeoQuery](https://aclanthology.org/P12-1051/)
- 🇮🇹 Italian, based on translations that were provided by two native speaker annotators as part of this work

The alignments were provided by expert annotators who found that the majority of the examples can be aligned monotonically.

*06-15-2022: English and Italian versions are now available. German to be uploaded shortly.*

## Format
The dataset can be found in the `data` folder and it comes in `.csv` format. There are five columns:
1. ID : contains the ids of the example
2. NL : contains the natural language queries
3. MR : contains the meaning representation programs
4. ALIGNMENT : contains the word alignments
5. MONOTONIC : contains labels indicating whether the alignment is monotonic

The `splits` folder contains listss of IDs for three different splits: a question split, a query split and a length split. The test set IDs are found in the `test.txt` files. Moreover, we provide three development sets `dev1.txt`, `dev2.txt` and `dev3.txt`, which can be used for validation.

## Citation
If you find GEO-Aligned useful in your research, please cite this paper:
```
@misc{https://doi.org/10.48550/arxiv.2205.08288,
  doi = {10.48550/ARXIV.2205.08288},
  url = {https://arxiv.org/abs/2205.08288},
  author = {Locatelli, Davide and Quattoni, Ariadna},
  title = {Measuring Alignment Bias in Neural Seq2Seq Semantic Parsers},
  publisher = {arXiv},
  year = {2022},
}
```
