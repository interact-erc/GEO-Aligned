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
The dataset comes in `.csv` format, and it has four columns:
1. NL : contains the natural language queries
2. MR : contains the meaning representation programs
3. ALIGNMENT : contains the word alignments
4. MONOTONIC : contains labels indicating whether the alignment is monotonic

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
