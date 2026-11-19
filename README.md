# Which Records Matter? Shapley-Based Data Valuation
 
**Tutorial Material**
 
Andreas Loizou · Nikolaos Andriotis · Dimitrios Tsoumakos
Database and Knowledge Systems Lab (DBLab), National Technical University of Athens
 
---
 
## About
 
Real-world data repositories are full of noisy, mislabeled, duplicated and irrelevant records, and training on such data degrades downstream models. Data valuation asks a simple question: **how much does each record contribute to a model or a query?** Shapley-based methods answer it with a principled, game-theoretic notion of contribution.
 
This tutorial surveys Shapley-based data valuation from a data management perspective. It covers exact and approximate estimators, semivalues and closed forms, techniques for scaling valuation to large repositories, and recent extensions to graph and multimodal data. It closes with use cases in the data management stack and open problems.
 
## Contents
 
| Folder | What it holds |
|---|---|
| [`Tutorial-Which_Records_Matter.pdf`](Tutorial-Which_Records_Matter.pdf) | Tutorial slides |
| `notebooks/` | Hands-on Colab notebooks (coming soon) |
| `reading-list.md` | Papers covered in the tutorial, grouped by part (coming soon) |
 
## Outline
 
| Part | Topic | Minutes | Presenter |
|---|---|---|---|
| I | Foundations and Leave-One-Out | 15 | A. Loizou |
| II | Sampling-based Shapley estimators | 10 | A. Loizou |
| III | Semivalues, closed forms and learner-free valuation | 20 | A. Loizou |
| IV | Scaling valuation to repositories | 15 | A. Loizou |
| V | Beyond tabular data: graphs and multimodal | 18 | N. Andriotis |
| VI | Data management use cases and open problems | 12 | D. Tsoumakos |
 
The 3-hour version adds 45 minutes of depth (slides marked "3-hour version") and a 45-minute hands-on session.
 
## Methods covered
 
- **Foundations:** Leave-One-Out, influence functions, Shapley values of facts in query answering
- **Sampling-based estimators:** TMC-Shapley, G-Shapley
- **Semivalues and closed forms:** Beta-Shapley, Data Banzhaf, kNN-Shapley, Threshold kNN-Shapley
- **Learner-free valuation:** Data-OOB, LAVA
- **Scaling:** In-Run Data Shapley, DataScope, DVRL, 2D-Shapley, C-DaSh
- **Graphs:** PC-Winter, SGUL
- **Multimodal and related attribution:** MM-SHAP, Shap-CA, TRAK, DataInf, LESS
## Hands-on session
 
The notebooks run on Google Colab and use [OpenDataVal](https://github.com/opendataval/opendataval) and [pyDVL](https://github.com/aai-institute/pyDVL). You will:
 
1. Inject label noise into a small public dataset.
2. Run LOO, TMC-Shapley, Beta-Shapley, Data Banzhaf, kNN-Shapley, Data-OOB and C-DaSh.
3. Compare noisy-label detection and point-removal curves across estimators.
No local installation is needed; open a notebook in Colab and run the cells in order.
 
## Contact
 
{antreasloizou, nandriotis, dtsouma}@mail.ntua.gr
