# NTUA AI Coursework

**Student:** Michael-Athanasios Peppas (03121026)
**Institution:** National Technical University of Athens, ECE

This repository includes Google Colab notebooks from four NTUA ECE courses: Artificial Intelligence, Machine Learning, Neural Networks & Deep Learning, and Image and Video Technology and Analysis. Each course contains two comprehensive lab projects with supporting code, data, references, and experiment notes.

---

## Courses

### Artificial Intelligence

- **AI_Lab1:** Maze generation, search algorithms (BFS, Dijkstra, A*, Greedy), and adversarial planning with Alpha-Beta agents.
- **AI_Lab2:** Hybrid movie recommender combining SWI-Prolog symbolic reasoning and Python for data handling and evaluation.

See `Artificial_Intelligence/README.md` for detailed instructions, key concepts, and results.

### Machine Learning

- **ML_Lab1:** RainTomorrow classification: data preprocessing, feature engineering, model training with scikit-learn, and evaluation.
- **ML_Lab2:** Salinas hyperspectral clustering and classification using KMeans, Fuzzy C-Means, PCA, and CNN feature extraction.

See `Machine_Learning/README.md` for detailed instructions, key concepts, and results.

### Neural Networks & Deep Learning

- **DL_Lab1:** WideResNet architectures on CIFAR-10, Mixup augmentation, calibration measurement, and robustness on CIFAR-10-C.
- **DL_Lab2:** Transformer fine-tuning for sentiment, PiQA, TruthfulQA, and Winogrande tasks using Hugging Face.

See `Neural_Networks_and_Deep_Learning/README.md` for detailed instructions, key concepts, and results.

### Image and Video Technology and Analysis

- **Lab 1:** Laplacian pyramid image coding with Gaussian/Laplacian pyramid construction, exact reconstruction, entropy analysis, and quantization experiments.
- **Lab 2:** CNN image classification on a 20-class CIFAR-100 subset using LeNet, AlexNet, VGG, MyCNN, dropout/data augmentation, VGG19, and EfficientNetB0.

See `Image_and_Video_Technology_and_Analysis/README.md` for detailed instructions, key concepts, and results.

---

## Repository Structure

```bash
ntua-ai-coursework/
├── Artificial_Intelligence/
│   ├── AI_Lab1/
│   ├── AI_Lab2/
│   └── README.md
├── Machine_Learning/
│   ├── ML_Lab1/
│   ├── ML_Lab2/
│   └── README.md
├── Neural_Networks_and_Deep_Learning/
│   ├── DL_Lab1/
│   ├── DL_Lab2/
│   └── README.md
├── Image_and_Video_Technology_and_Analysis/
│   ├── lab1/
│   ├── lab2/
│   ├── lab_material/
│   └── README.md
├── docs/
│   └── project_structure/
├── LICENSE
└── README.md
```

---

## Setup and reproducibility

The courses use distinct runtimes. Read the selected course README and notebook setup cells before preparing an environment; a single bulk installation does not reproduce all eight exercises. Exact historical package versions are not frozen in this repository.

| Course | Runtime/input considerations |
| --- | --- |
| Artificial Intelligence | AI Lab 1 is a Colab-link text artifact; its external notebook is not versioned here. AI Lab 2 combines Python, SWI-Prolog and `pyswip`. |
| Machine Learning | Python/scikit-learn tabular and hyperspectral workflows; keep the supplied CSV/NumPy inputs adjacent to each notebook. CNN feature experiments need their declared numerical framework. |
| Neural Networks & Deep Learning | PyTorch/Hugging Face notebooks, external datasets/model downloads and GPU memory requirements; DL Lab 1 additionally uses CIFAR-10-C. |
| Image and Video Technology and Analysis | Image processing and CNN notebooks with their own data/model paths and framework requirements. |

```bash
GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/ntua-el21026/NTUA-AI_Coursework.git
cd NTUA-AI_Coursework
```

For execution, use the notebook's intended Colab/Jupyter environment, inspect its setup cells, and install only the selected lab's dependencies. Reuse a compatible managed PyTorch/CUDA stack; the repository review does not require installing one locally. Keep support folders beside each notebook. Record actual Python/package/GPU versions, seeds, data/model hashes and the source revision. Write rerun notebooks and generated results to separate storage so submitted evidence remains intact.

## Evidence and limitations

The repository supports a portfolio of coursework implementations by Michail-Athanasios Peppas (03121026). Embedded reports, third-party starter material and referenced work retain their original attribution. This does not establish sole authorship of course designs, datasets or pretrained models.

Stored outputs describe historical executions. Some notebooks have outputs with null execution counts; that weakens replay provenance and does not establish non-execution. The IVTA classifier selects a model using test macro-F1, so those comparisons are exploratory coursework selection, not an untouched confirmation test. The ML Lab 2 notebook says 2023–24 while the course README says 2024–25; completion dates require confirmation before use in an application. No training or independent numerical replay was run during portfolio preparation.

## Publication status and asset scope

This remains a conditional public portfolio candidate. Markdown cell 1 (zero-based) of both `Machine_Learning/ML_Lab1/ML_Lab1.ipynb` and `Machine_Learning/ML_Lab2/ML_Lab2.ipynb` explicitly prohibits posting laboratory solutions on GitHub or other websites and attributes project design/content to the teaching team. Those notices and all submitted solutions/outputs are preserved. A public release containing those solutions requires an applicable documented permission; this preparation contacted no instructors and did not treat removal of notices or coursework as a remedy.

Course slides, handouts, papers, templates, datasets and model assets need individual attribution/redistribution review. The MIT notice governs original contributions only within the contributors' rights; it does not override course restrictions or third-party terms. Public-first curation can proceed for material with established permission while retaining this complete local evidence copy.

---

## License

Original contributions are offered under MIT to the extent their authors hold the relevant rights. See `LICENSE` and the publication/asset scope above.

---

## *Prepared by Michael-Athanasios Peppas (03121026)*
