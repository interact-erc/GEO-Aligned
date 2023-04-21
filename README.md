# GEO-Aligned

## Introduction
GEO-Aligned is a semantic parsing dataset that was obtained by augmenting the popular GeoQuery data with word alignment information. You can read about it in our *SEM [paper](https://aclanthology.org/2022.starsem-1.17/).

It comes in three languages:
- English, based on the [original dataset](https://dl.acm.org/doi/10.5555/1864519.1864543)
- German, based on [multilingual GeoQuery](https://aclanthology.org/P12-1051/)
- Italian, based on translations that were provided by two native speaker annotators as part of this work

The alignments were provided by expert annotators who found that the majority of the examples can be aligned monotonically.

## Format
The dataset can be found in the `data` folder and it comes in `.csv` format. There are five columns:
1. ID : contains the ids of the example
2. NL : contains the natural language queries
3. MR : contains the meaning representation programs
4. ALIGNMENT : contains the word alignments
5. MONOTONIC : contains labels indicating whether the alignment is monotonic

There are two versions for each language: 
- Files named `{language}.csv` contain the dataset with constants (city names, state names, etc)
- Files named `{language}_anon.csv` contain the anonymized version of the data

The `splits` folder contains lists of IDs for three different splits: a question split, a query split and a length split. The test set IDs are found in the `test.txt` files. Moreover, we provide three development sets `dev1.txt`, `dev2.txt` and `dev3.txt`, which can be used for validation.

## Citation
If you find GEO-Aligned useful in your research, please cite this paper:
```
@inproceedings{locatelli-quattoni-2022-measuring,
    title = "Measuring Alignment Bias in Neural Seq2seq Semantic Parsers",
    author = "Locatelli, Davide  and
      Quattoni, Ariadna",
    booktitle = "Proceedings of the 11th Joint Conference on Lexical and Computational Semantics",
    month = jul,
    year = "2022",
    address = "Seattle, Washington",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.starsem-1.17",
    doi = "10.18653/v1/2022.starsem-1.17",
    pages = "200--207"
}
```
