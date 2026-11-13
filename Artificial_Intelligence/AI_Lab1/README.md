# AI Lab 1: Maze Search and Adversarial Planning

[AI_Lab1.ipynb](AI_Lab1.ipynb) is the authentic `AI_25_03121026.ipynb` retrieved from the [original Colab source](https://colab.research.google.com/drive/1FvRNBpS0JBHY_WgzuzQOtq8fq7hSPGJG?usp=sharing) on 13 November 2026. It contains 86 cells: 48 Markdown and 38 code cells. The source download was 8,171,951 bytes with SHA-256 `7e4302dfffcbc630a8766fecaa1275329d20cc2d98eb8ccb59b1dba66679ac3c`; a second independent download matched exactly.

## Contents

The notebook implements maze generation, parameterized priority-queue search, heuristic comparisons, animated search traces, Alpha-Beta agents pursued by a ghost, and manually designed bonus mazes. Most implementation code is defined in the notebook itself. [AI_Lab1_utils/](AI_Lab1_utils/) contains `5.1.png` through `5.5.png`. All five are 301 × 301 PNGs and match the corresponding image bytes embedded in the original drawing-cell outputs.

[provenance.json](provenance.json) records both notebook hashes, image hashes/sizes, and three changed cells (zero-based):

- Cell 63 reads the default drawing from `drawing.png` in the working directory.
- Cell 68 describes repository image access.
- Cell 69 sets `maze_folder = 'AI_Lab1_utils/'`, replacing the personal Google Drive mount and absolute maze path.

All other source, metadata, execution counts, outputs, and the final AI-use disclaimer are preserved. Output messages still describe the historical executions, including the former Drive mount; the notebook has not been re-executed after these path changes. The original course instructions remain included and are not claimed as independently authored material.

## Local Jupyter

Use a Python environment with JupyterLab, NumPy, pandas, Matplotlib, and Pillow. From the repository root:

```bash
cd Artificial_Intelligence/AI_Lab1
python3 -m jupyter lab AI_Lab1.ipynb
```

Keep the kernel working directory at this lab directory. Parts 1–4 use ordinary Python/IPython libraries. The bonus drawing UI imports `google.colab.output.eval_js` in cell 62 and requires Colab. For local inspection of the existing bonus mazes, skip that drawing cell and the `draw(...)` calls in cells 71, 74, 77, 80, and 83; run `import PIL.Image` before the `draw_grid` definition, then use the supplied PNGs through `maze_folder`. This permits loading the archived maps without recreating the Colab drawing UI.

The notebook includes repeated randomized studies (including 120 mazes per size in one search comparison), so execute selected cells deliberately. A full run is not a quick installation check.

## Google Colab

Upload this lab directory with its `AI_Lab1_utils/` folder, or clone the repository in a Colab runtime:

```python
!git clone --depth 1 https://github.com/ntua-el21026/ntua-ai-coursework.git
%cd /content/ntua-ai-coursework/Artificial_Intelligence/AI_Lab1
```

Open the repository notebook in Colab or upload `AI_Lab1.ipynb`, then keep the runtime's working directory as shown above. The local maze path does not require Drive access. Execute drawing cells interactively only when creating new maps. Existing comparison cells load the preserved images; drawing new files in the current directory does not replace those archive inputs.

## Interpreting the evidence

The stored results are historical, with incomplete seed/runtime provenance. Some output-bearing code cells have null execution counts. The algorithm labeled BFS uses coordinate-ordered `PriorityQueue` ties with zero edge costs, rather than a FIFO BFS queue; its naming and accompanying claims remain preserved in the original submission. New correctness or performance conclusions require separate verification. No experiment or numerical test was run during integration.

The repository [authorship and licensing notes](../../README.md#authorship-publication-and-licensing) apply. No posting prohibition was identified in this retrieved notebook; that observation does not grant rights to third-party course content.
