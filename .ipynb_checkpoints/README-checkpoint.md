# patient_treatment_classification
Uses Kaggle dataset with real Indonesia hospital EHR records to test multiple predictive models for determining in-care or out-care.

Source: https://www.kaggle.com/datasets/saurabhshahane/patient-treatment-classification#

## Main Findings:

The following was the basis for the mutli-pipeline grid search component of this notebook: https://ryan-reilly.medium.com/gridsearch-pipelines-of-multiple-models-on-multiclass-classification-e9124b6ea2e3

The goal was to test multiple models, both simple and more sophisticated, to see which would perform best. Random Forest performed as well if not slightly better than XGBoost, with a top accuracy of ~75%. Data was cleaned beforehand to account for the class imbalance, with a random subset taken out of the original dataset to even the class sizes.