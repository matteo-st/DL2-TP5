# DL2 — TP5: Adversarial Examples (*Importance of Git*)

Deep Learning II — Université Paris Dauphine-PSL.

The subject is in **[TP5.pdf](TP5.pdf)**. Read it first.

## Getting started

This repository is a **template**: you cannot push to it. Create your own copy first:

1. Click **Use this template → Create a new repository** (top of this page) and create it under your account, e.g. `DL2-TP5`.
2. Clone **your** repository:
   ```bash
   git clone https://github.com/<your-username>/DL2-TP5.git
   cd DL2-TP5
   ```
3. Set up the environment with one of the files in `config/`:
   ```bash
   # conda
   conda env create -f config/environment.yml
   # or pip / virtualenv
   pip install -r config/requirements.txt
   ```

GitHub does not accept your password for `git push`: authenticate once with `gh auth login` (GitHub CLI), a personal access token, or an SSH key.

## Files

| File | Content |
|---|---|
| `train.py` | Trains a model on CIFAR-10 |
| `evaluate.py` | Evaluates a trained model under an adversarial attack |
| `run_xp.py` | Runs several evaluations in a row |
| `models.py` | Model definitions (FC, CNN, ResNet18) |
| `attack_utils.py` | FGSM and PGD attacks |
| `utils.py` | Training, evaluation and plotting helpers |
