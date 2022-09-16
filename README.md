# EvoTorch Baseline for Myosuite Challenge

This repository contains resources implementing an [EvoTorch](evotorch.ai) baseline for the [Myosuite Challenge](https://sites.google.com/view/myochallenge).

## Table of Contents

* [Installation](#installation)
* [Training](#training)
* [Visualization](#visualization)
* [Submission](#submisssion)
* [Authors](#authors)

## Installation

The easiest way to use these resources is to have [conda](https://docs.conda.io/en/latest/miniconda.html) installed. Then you can run:

```bash
git clone TODO:LINKTOGIT
cd TODO:PATHTOFOLDER
conda env create -f env.yml
conda activate myosuite-challenge
jupyter notebook
```

## Training

To begin training, open `train.ipynb` and step through the existing code blocks. This should train an agent for the Boading challenge!

## Visualization

To visualize, first run training. Then you should have saved learned policies in your local directory. If you have done this, you can open `visualize.ipynb` and step through the existing code blocks to visualize the learned behaviours and get estimations of performance metrics.

## Submission

To submit, follow the instructions at https://github.com/ET-BE/myoChallengeEval. We've provided a modified `agent_bb.py` file for you to place into `agent/` of your local clone of the official submission repo (replacing the existing demo `agent_bb.py`). Then simply copy `learned_policy_boading.pkl` to the `agent/policies/` folder and you should be good to submit!

While following the instructions for submission, we recommend that you create a new `conda` environment to avoid mixing dependencies:

```bash
conda deactivate
conda create -n myosuite-submit
conda activate myosuite-submit
...
```

## Authors

- [**Timothy Atkinson**](mailto:timothy@nnaisense.com)
- [**Nihat Engin Toklu**](mailto:engin@nnaisense.com)
