# Machine Learning

Two individual NTUA coursework notebooks by **Michail-Athanasios Peppas (03121026)**. Both retain Greek assignment text, implementations, recorded outputs, and the teaching team's publication notices.

## Labs and supplied inputs

| Lab | Work implemented | Supplied files |
| --- | --- | --- |
| [Lab 1](ML_Lab1/ML_Lab1.ipynb) | RainTomorrow classification; missing-value handling, preprocessing, classifier comparisons, grid search, and test predictions | [ML_Lab1_utils/](ML_Lab1/ML_Lab1_utils/): `train-val.csv`, `test.csv` |
| [Lab 2](ML_Lab2/ML_Lab2.ipynb) | Salinas hyperspectral clustering with KMeans, PCA, and fuzzy C-means; EuroSAT image clustering/feature experiments with MobileNetV3Small | [ML_Lab2_utils/](ML_Lab2/ML_Lab2_utils/): `salinas_image.npy`, `salinas_labels.npy` |

Lab 1 compares scikit-learn classifiers including logistic regression, Gaussian naive Bayes, K-nearest neighbors, decision trees, random forests, SVMs, and MLPs. Lab 2 evaluates cluster assignments using adjusted Rand scores and silhouette measures where applicable. Numerical comparisons and their settings are recorded in the notebooks; no new results are asserted by this guide.

## Running a copy

```bash
git clone https://github.com/ntua-el21026/ntua-ai-coursework.git
cd ntua-ai-coursework/Machine_Learning
```

Use a separate environment for the chosen notebook. Common libraries include NumPy, pandas, Matplotlib, seaborn, and scikit-learn. Lab 2 imports `FCM` from the **`fuzzy-c-means`** package and TensorFlow/Keras for the image-feature section; `scikit-fuzzy` is not the imported FCM dependency.

The submitted notebooks load the CSV/NumPy filenames from the current working directory, while Git stores those inputs in the adjacent utility folders. In a rerun copy, either copy the supplied inputs beside the notebook or adapt the file references to the utility directory. Inspect cells before execution: Lab 2 downloads/extracts EuroSAT into `2750/` and obtains pretrained weights; those large third-party assets are not versioned here. Historical download cells disable certificate checks; obtain and verify the dataset through an authorized trusted source when preparing a new run.

Lab 1 writes `submission_nopt_fin.csv` and `submission_opt_fin.csv` to the working directory. Keep new predictions and outputs separate from the original evidence. Exact package versions and a complete historical environment lock are not available.

## Evidence and publication limits

Both notebooks explicitly prohibit posting laboratory solutions on GitHub or other websites in Markdown cell 1 (zero-based), and credit the teaching team for project design/content. The notices and submitted work are preserved. An applicable documented permission is required to redistribute the restricted material publicly; repository visibility does not establish permission.

Lab 1's header names academic year 2024–25; Lab 2's header names 2023–24. This discrepancy remains unresolved, so a common completion year is not asserted. Recorded metrics have not been independently replayed during documentation preparation.

The root [MIT license](../LICENSE) applies only to original contributions within the authors' rights. See the [asset inventory](../docs/ASSETS.md) for external datasets and the repository [publication notes](../README.md#authorship-publication-and-licensing).
