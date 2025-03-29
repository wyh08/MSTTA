# MSTTA
A Model Selection-Based Test-time Data Augmentation Method

To reproduce the experimental results of the MSTTA method, please execute the following code files in sequence:

    1.Labeling_Roberta_model.ipynb - Fine-tune RoBERTa to train a labeling model

    2.train_aug_labeling.ipynb - Annotate optimal and suboptimal augmentation methods for train/test sets

    3.Test_aug_select_model.ipynb - Train a classifier to predict best augmentation methods for test instances

    4.traditional_enhanced.ipynb - Traditional augmentation (fixed two methods)

    5.random_enhanced.ipynb - Random augmentation (randomly select two methods)

    6.enhanced_test.ipynb - Apply selected augmentation strategies to test set

    7.Compare.ipynb - Perform uncertainty-weighted prediction and result comparison

    8.Models/ - Benchmark with different inference models

    9. verify/ - Validation experiment (non-practical scenario):
        Run sequentially: test_aug_labeling.ipynb → enhanced_test.ipynb → Compare.ipynb
        Note: Copy the trained labeling model from Step 1 to this directory first
