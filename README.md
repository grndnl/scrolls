# SCROLLS

This repository contains the official code of the paper: ["SCROLLS: Standardized CompaRison Over Long Language Sequences"](https://arxiv.org/abs/2201.03533).

Setup instructions are in the [baselines](https://github.com/tau-nlp/scrolls/tree/main/baselines)   and [evaluator](https://github.com/tau-nlp/scrolls/tree/main/evaluator)   folders. 

For the live leaderboard, checkout the [official website](https://scrolls-benchmark.com/). 

***
## Loading the SCROLLS Benchmark Datasets
- via [🤗 Datasets (huggingface/datasets)](https://github.com/huggingface/datasets) library (recommended):

    1. [Installation](https://github.com/huggingface/datasets#installation)
    2. Usage:

        ```python
        from datasets import load_dataset

        qasper_dataset = load_dataset("tau/scrolls", "qasper")
        """
        Options are: ["gov_report", "summ_screen_fd", "qmsum", "narrative_qa", "qasper", "quality", "contract_nli"]
        """
        ```
- via ZIP files, where each split is in a JSONL file:
  - [GovReport](https://scrolls-tau.s3.us-east-2.amazonaws.com/gov_report.zip)
  - [SummScreenFD](https://scrolls-tau.s3.us-east-2.amazonaws.com/summ_screen_fd.zip)
  - [QMSum](https://scrolls-tau.s3.us-east-2.amazonaws.com/qmsum.zip)
  - [NarrativeQA](https://scrolls-tau.s3.us-east-2.amazonaws.com/narrative_qa.zip)
  - [Qasper](https://scrolls-tau.s3.us-east-2.amazonaws.com/qasper.zip)
  - [QuALITY](https://scrolls-tau.s3.us-east-2.amazonaws.com/quality.zip)
  - [ContractNLI](https://scrolls-tau.s3.us-east-2.amazonaws.com/contract_nli.zip)


## Citation
```
@inproceedings{shaham-etal-2022-scrolls,
    title = "{SCROLLS}: Standardized {C}ompa{R}ison Over Long Language Sequences",
    author = "Shaham, Uri  and
      Segal, Elad  and
      Ivgi, Maor  and
      Efrat, Avia  and
      Yoran, Ori  and
      Haviv, Adi  and
      Gupta, Ankit  and
      Xiong, Wenhan  and
      Geva, Mor  and
      Berant, Jonathan  and
      Levy, Omer",
    booktitle = "Proceedings of the 2022 Conference on Empirical Methods in Natural Language Processing",
    month = dec,
    year = "2022",
    address = "Abu Dhabi, United Arab Emirates",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2022.emnlp-main.823",
    pages = "12007--12021",
}
```
When citing SCROLLS, please make sure to cite all of the original dataset papers. [[bibtex]](https://scrolls-tau.s3.us-east-2.amazonaws.com/scrolls_datasets.bib)
