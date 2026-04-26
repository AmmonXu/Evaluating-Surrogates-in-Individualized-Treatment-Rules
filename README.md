# Evaluating-Surrogates-in-Individualized-Treatment-Rules

Reproducible code for simulation and application in the article "Evaluating Surrogates in Individualized Treatment Rules".

**For Application:**

* `criteo-uplift-v2.1.csv`: this dataset contains the Criteo uplift data used in the application.
  * The dataset is available at this link: [https://ailab.criteo.com/criteo-uplift-prediction-dataset/](https://ailab.criteo.com/criteo-uplift-prediction-dataset/).

* Application code is organized within the `no_bootstrap` directory, categorized by different machine learning models (`boosting`, `kernelr`, `lightGBM`, `rbf`, `xgboost`).
  * Inside each model's folder, there are specific scripts for different outcomes (e.g., `xgb_exposure.py` and `xgb_visit.py`).
  * **Note:** To reproduce all the results presented in the application under different budget constraints, you need to manually modify the `lambda_val` parameter within these scripts to correspond to the specific budget.

**For Simulation:**

* Simulation code for evaluating measures with and without budget constraints:
  * `no_quantile_simulation.py`: main code for evaluation measures simulation without budget constraints.
  * `quantile_simulation.py`: main code for evaluation measures simulation with budget constraints.

*** 

**提示：** 您可以将 `[Your Article Name Here]` 替换为您实际的论文或项目名称。如果需要进一步细化模型文件夹的说明，也可以根据需要随时调整。
