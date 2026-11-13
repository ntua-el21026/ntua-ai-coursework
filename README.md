# NTUA AI Coursework

Eight laboratory submissions by **Michail-Athanasios Peppas (03121026)** for the NTUA School of Electrical and Computer Engineering. The collection covers classical search, symbolic recommendation, machine learning, deep learning, and image analysis. Notebooks retain their explanations and recorded outputs; the repository is an academic archive with lab-specific execution requirements.

## Coursework index

| Course | Lab | Implementation and evidence |
| --- | --- | --- |
| [Artificial Intelligence](Artificial_Intelligence/README.md) | 1 | [Maze generation, priority-queue search variants, and adversarial Alpha-Beta agents](Artificial_Intelligence/AI_Lab1/AI_Lab1.ipynb); [execution and provenance notes](Artificial_Intelligence/AI_Lab1/README.md) |
| Artificial Intelligence | 2 | [Python/SWI-Prolog movie recommender](Artificial_Intelligence/AI_Lab2/AI_Lab2.ipynb), with [rules and CSV inputs](Artificial_Intelligence/AI_Lab2/AI_Lab2_utils/) |
| [Machine Learning](Machine_Learning/README.md) | 1 | [RainTomorrow classification](Machine_Learning/ML_Lab1/ML_Lab1.ipynb): preprocessing, classifier comparison, and model selection |
| Machine Learning | 2 | [Salinas hyperspectral clustering and EuroSAT feature experiments](Machine_Learning/ML_Lab2/ML_Lab2.ipynb) |
| [Neural Networks and Deep Learning](Neural_Networks_and_Deep_Learning/README.md) | 1 | [WideResNet, Mixup, calibration, and CIFAR-10-C evaluation](Neural_Networks_and_Deep_Learning/DL_Lab1/DL_Lab1.ipynb); helper code and large artifacts remain external |
| Neural Networks and Deep Learning | 2 | [Transformer workflows for Yelp Polarity, PiQA, TruthfulQA, and Winogrande](Neural_Networks_and_Deep_Learning/DL_Lab2/DL_Lab2.ipynb) |
| [Image and Video Technology and Analysis](Image_and_Video_Technology_and_Analysis/README.md) | 1 | [Gaussian/Laplacian pyramids, reconstruction, entropy, and quantization](Image_and_Video_Technology_and_Analysis/lab1/IVTA_03121026_Peppas_Michael_1.ipynb) |
| Image and Video Technology and Analysis | 2 | [CIFAR-100 subset CNN comparison, regularization, and transfer learning](Image_and_Video_Technology_and_Analysis/lab2/IVTA_03121026_Peppas_Michael_2.ipynb) |

[Image-analysis teaching notebooks](Image_and_Video_Technology_and_Analysis/lab_material/) and the original papers, handouts, templates, and supplied data provide context. They retain their respective authorship and rights.

## Inspection and execution

```bash
GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/ntua-el21026/ntua-ai-coursework.git
cd ntua-ai-coursework
```

Read the selected course README and notebook setup cells before preparing an environment. There is no common dependency lock or repository-wide test runner. AI Lab 1 is now included with its five original maze images; its [provenance record](Artificial_Intelligence/AI_Lab1/provenance.json) identifies the independently retrieved source and the limited asset-path changes.

The other submitted notebooks retain historical paths. For a rerun, work on a copy and map the supplied inputs to the filenames expected by that notebook. Managed Colab is appropriate for GPU workloads; reuse a compatible provider PyTorch/CUDA stack. Local Jupyter is suitable where the notebook's libraries and platform-specific cells permit it. Do not assume every notebook supports an unchanged local “Run all”. See the [asset and portability inventory](docs/ASSETS.md) for missing helpers, external downloads, and required paths.

Record Python/package versions, hardware, seeds, data/model hashes, and the source revision for a new execution. Store rerun notebooks, checkpoints, and generated results separately from the submitted evidence. Training and full experiment sweeps are substantial workloads.

## Evidence and limitations

Recorded notebook outputs are the source for coursework results. They have not been independently numerically replayed during documentation preparation. Some output-bearing cells have null execution counts, and the historical environments are not fully frozen. The IVTA classifier selects configurations using test macro-F1; those comparisons are exploratory model selection, rather than an untouched confirmation test. ML Lab 2's header names 2023–24 while the earlier course overview named 2024–25; the completion year remains unresolved.

AI Lab 1 preserves its original algorithm names and conclusions. In particular, the combination labeled BFS uses a `PriorityQueue` with coordinate-based tie ordering and zero edge cost; it is not a conventional FIFO BFS implementation. The original work has not been changed to resolve that distinction.

## Authorship, publication, and licensing

The submissions identify Michail-Athanasios Peppas; assignment designs, starter code, teaching materials, datasets, pretrained models, and cited papers retain their original attribution. AI-use disclosures in the notebooks remain intact.

Both Machine Learning notebooks explicitly prohibit posting laboratory solutions on GitHub or other websites and attribute the project design/content to the teaching team (Markdown cell 1, zero-based). Those notices and submissions are preserved. An applicable documented permission is required for public redistribution of that material. Repository visibility is not evidence of such permission.

Course slides, handouts, papers, templates, datasets, and model assets require individual rights review. The [MIT license](LICENSE) covers original contributions only to the extent their authors hold the relevant rights; it does not override course restrictions or third-party terms.
