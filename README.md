# Multimodal Belief

This is the repository corresponding to [Multimodal Belief Prediction](https://www.isca-archive.org/interspeech_2024/murzaku24_interspeech.html), which was accepted to Interspeech 2024. It contains the code and data used for our unimodal baseline experiments as well as our multimodal fusion runs.

## Installation
Supposing [conda](https://docs.conda.io/en/latest/) and [poetry](https://python-poetry.org) are installed, the project dependencies can be setup using the following commands.

```
conda create -n multimodal-belief python=3.10
conda activate multimodal-belief
poetry install
```

By default, all scripts will log their output to `/home/{username}/scratch/logs/`. To change this behavior see ~line 40 of `src/core/context.py`.

## Content
A summary of the content and structure of the repository is shown below.

```
multimodal-belief/
|- bin/
|  |- multimodal_classification.py - runs classification experiments.
|- configs/                        - example training configurations.
|- data/cb/                        - commitment bank data.
|- src/
|  |- ...                          - additional utilities and code.
```

## Citation

```
@inproceedings{murzaku24_interspeech,
  title     = {Multimodal Belief Prediction},
  author    = {John Murzaku and Adil Soubki and Owen Rambow},
  year      = {2024},
  booktitle = {Interspeech 2024},
  pages     = {1075--1079},
  doi       = {10.21437/Interspeech.2024-2103},
  issn      = {2958-1796},
  url       = {https://www.isca-archive.org/interspeech_2024/murzaku24_interspeech.html}
}
```
