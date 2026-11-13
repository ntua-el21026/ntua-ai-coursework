# Artificial Intelligence

Two NTUA laboratory submissions by **Michail-Athanasios Peppas (03121026)**. The notebooks contain implementation, analysis, and historical outputs; the original course instructions and AI-use disclosures remain part of the submissions.

## Lab 1: maze search and adversarial agents

Open [AI_Lab1.ipynb](AI_Lab1/AI_Lab1.ipynb). It implements a randomized DFS-style maze generator, a parameterized priority-queue pathfinder, Manhattan/Euclidean/Chebyshev/Octile heuristics, search visualizations, and Alpha-Beta ghost-avoidance experiments. A bonus section uses five manually drawn mazes and a hill-climbing agent.

The implementation is inside the notebook. [AI_Lab1_utils/](AI_Lab1/AI_Lab1_utils/) contains five PNG images, rather than separate Python helper modules. The notebook was independently retrieved from the original Colab link and integrated with limited local asset-path corrections. See the [Lab 1 guide](AI_Lab1/README.md) for local/Colab use and [provenance.json](AI_Lab1/provenance.json) for hashes and the exact change scope.

Stored labels and conclusions are historical coursework evidence. The zero-cost/zero-heuristic variant labeled BFS uses priority-queue tie ordering rather than a FIFO queue. No new optimality, timing, or win-rate result is claimed here.

## Lab 2: hybrid movie recommendation

Open [AI_Lab2.ipynb](AI_Lab2/AI_Lab2.ipynb). Python reads movie metadata, asserts facts into SWI-Prolog through `pyswip`, and combines symbolic movie similarities with user ratings. The notebook includes tiered similarity schemes, caching, parameter comparisons, and precision/recall/F1 evaluation.

[AI_Lab2_utils/](AI_Lab2/AI_Lab2_utils/) includes `db.pl`, `movies_metadata.csv`, `train_ratings.csv`, and `test_ratings.csv`. Recommendation logic is in notebook cells; there is no separate `recommender.py` module.

Requirements include Python, NumPy, pandas, Matplotlib, scikit-learn, tqdm, `pyswip`, and an installed SWI-Prolog runtime. The notebook contains Colab installation and Drive cells, and repeats the original personal Drive path in several places. For a local copy, skip the Drive-mount cell, set each `path` assignment to the resolved `AI_Lab2_utils/` directory with a trailing separator, and consult the supplied `db.pl` as described in the notebook. For Colab, upload the same files or clone the repository and use its corresponding runtime path. Preserve the submitted notebook when adapting paths for a rerun.

## Reproducibility

The labs use different dependencies and are not distributed as an installable package or a locked environment. Inspect setup cells before execution and record actual versions, seeds, and input hashes. Run experiments on a copy and retain the original outputs.
