# Neural Networks and Deep Learning

NTUA laboratory notebooks by **Michail-Athanasios Peppas (03121026)**, preserving training/evaluation code, discussion, and recorded outputs. The two labs have distinct data and model requirements.

## Lab 1: WideResNet and Mixup

[DL_Lab1.ipynb](DL_Lab1/DL_Lab1.ipynb) studies WideResNet configurations (WRN-40-4, WRN-28-10, and WRN-16-8), dropout, Mixup, classification accuracy, calibration, and robustness on CIFAR-10-C. It imports a separate `wideresnet.py` and contains data-loading, training, checkpoint, and evaluation routines.

The committed [DL_Lab1_Utils/utils_link.txt](DL_Lab1/DL_Lab1_Utils/utils_link.txt) points to the original Google Drive folder. **The helper module, weights, datasets, logs, and runs are not present in the Git tree.** The folder listing was accessible during documentation preparation and included `wideresnet.py`, `cifar/`, `data/`, `models/`, and `runs/`. The small module was inspectable, but its course/upstream distribution rights were not established, so it remains external. Do not infer that all linked weights or datasets have been downloaded or verified.

For a legitimate rerun, obtain the course helper through the linked folder and preserve its provenance. The historical cells repeatedly expect a Drive working folder at `/content/drive/My Drive/NTUA-NNDL/Lab_DL_ex1`, with `wideresnet.py` on `sys.path`, CIFAR-10 data, a `models/` directory, and `runs/`. CIFAR-10-C arrays are expected under `data/cifar/CIFAR-10-C/`, including `labels.npy` and the corruption `.npy` files. The notebook also accesses `data/cifar/cifar-10-batches-py/`. Inspect all path assignments in a rerun copy rather than changing the preserved submission.

Requirements include a compatible PyTorch/torchvision environment, NumPy, pandas, Matplotlib, seaborn, and scikit-learn. The [CIFAR-10-C dataset](https://zenodo.org/records/2535967) is a large external input. Training and corruption evaluation need substantial compute/storage; recorded missing-file incidents and their discussion remain in the notebook.

## Lab 2: Transformer workflows

[DL_Lab2.ipynb](DL_Lab2/DL_Lab2.ipynb) uses Hugging Face pipelines and training tools for:

- Yelp Polarity sentiment classification and fine-tuning.
- PiQA comparisons based on natural-language-inference scores.
- TruthfulQA answer ranking with NLI and sentence embeddings.
- Winogrande experiments using masked language models, NLI, sequence classification, and text-to-text generation.

The notebook imports PyTorch, `transformers`, `datasets`, `evaluate`, `sentence-transformers`, NumPy, pandas, Matplotlib, seaborn, scikit-learn, tqdm, and tabulate. Datasets and pretrained models are downloaded externally; inspect the exact identifiers and selected sample sizes in each section. This is a collection of task-specific experiments, not a single trained model or deployed NLP service.

## Execution and evidence

```bash
GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/ntua-el21026/ntua-ai-coursework.git
cd ntua-ai-coursework/Neural_Networks_and_Deep_Learning
```

Open the chosen notebook in Colab or a suitably provisioned Jupyter environment. Lab 1 requires the external helper and path preparation described above. Reuse a compatible managed PyTorch/CUDA runtime and inspect notebook setup cells before installing only the selected lab's remaining dependencies. No exact historical dependency lock is provided, and changing framework versions can affect compatibility and numerical results.

Preserve the original notebooks and write new runs, downloads, checkpoints, and metrics separately. Record actual hardware, package versions, source/model/data hashes, seeds, and evaluation subsets. Stored metrics are historical coursework evidence; no training, model download, or numerical replay was performed for this documentation update. See the [asset inventory](../docs/ASSETS.md) for remaining external dependencies.

Original submissions retain their AI-use disclosures and academic attribution. The root [MIT license](../LICENSE) covers original contributions within the authors' rights; course helpers, datasets, pretrained models, and papers retain their own terms. See the repository [publication notes](../README.md#authorship-publication-and-licensing).
