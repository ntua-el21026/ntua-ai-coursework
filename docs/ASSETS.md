# Coursework assets and portability

This inventory distinguishes supplied files from external runtime dependencies. Original submissions, outputs, course notices, and third-party materials remain preserved. A successful file download does not establish redistribution rights.

| Lab | Available in this repository | External or runtime requirement |
| --- | --- | --- |
| AI 1 | [Notebook and five maze PNGs](../Artificial_Intelligence/AI_Lab1/README.md), including embedded historical animations/plots | Colab JavaScript bridge only for the interactive drawing UI. Personal Drive is no longer required for archived maze inputs. |
| AI 2 | Notebook, `db.pl`, movie metadata, train/test ratings | SWI-Prolog and `pyswip`; map repeated historical Drive `path` assignments to `AI_Lab2_utils/` in a rerun copy. Movie data retains its source rights. |
| ML 1 | Notebook, `train-val.csv`, `test.csv` | Notebook reads input basenames in its current directory. Supplied inputs are in `ML_Lab1_utils/`. |
| ML 2 | Notebook and Salinas `.npy` arrays | EuroSAT archive/extracted `2750/` images and MobileNetV3Small weights remain external third-party assets. Input `.npy` basenames are read from the current directory. |
| DL 1 | Notebook and original Drive-folder link | `wideresnet.py` remains external course helper code pending rights/provenance clearance. Linked CIFAR data, checkpoints, logs, and runs were not imported. CIFAR-10-C is available from its [dataset record](https://zenodo.org/records/2535967). |
| DL 2 | Notebook | Hugging Face datasets and pretrained models, network access, sufficient storage/memory, and their respective licenses/access terms. |
| IVTA 1 | Notebook, assignment, reference paper | Lena image is downloaded or supplied manually as `lena.png`; camera image comes from scikit-image. Image/paper rights remain separate. |
| IVTA 2 | Notebook, original template, assignment, reference papers, theory notes | CIFAR-100 and pretrained weights; class-selection/label tables hosted on Pastebin; original `q1_grid_results.csv` for resuming Q2 without rerunning Q1. |

## AI Lab 1 integration

The original source was independently downloaded twice from the ID in `AI_Lab1.txt`. Both downloads matched in size and SHA-256. Structure, metadata, code/Markdown source, text/HTML outputs, image payloads, and the AI-use disclosure were reviewed without executing the notebook. Author identity and historical Colab execution metadata were retained; no credential pattern was identified. The five existing PNGs match the notebook's original drawing outputs exactly. Only three asset-access cells were changed; all other source and all recorded outputs/counts/metadata are preserved. The [provenance record](../Artificial_Intelligence/AI_Lab1/provenance.json) provides the original and repository hashes plus image fingerprints.

## Remaining external material

The [DL Lab 1 Drive folder](https://drive.google.com/drive/folders/1Er6mi5njuZraQb7r9DknXDmBPM4uGjCM?usp=sharing) was accessible on 13 November 2026. Its listing contains the helper module and folders for data, weights, and runs. The retrieved helper's file-level text did not establish a redistribution grant or complete upstream attribution; it was therefore not added. The linked artifact collection was not downloaded in bulk. Exact checkpoint/data identity and access can only be established after obtaining and hashing those inputs.

Official dataset/model sources, academic citations, and library references remain legitimate external dependencies. No datasets or weights were fabricated, no frozen outputs were replaced, and no training was performed. ML publication restrictions are explicit in the original notebooks and are summarized in the [root README](../README.md#authorship-publication-and-licensing).
