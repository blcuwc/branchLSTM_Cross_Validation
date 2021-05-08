# branchLSTM_Cross_Validation
This project is a 5-fold cross validation experiment to original branchLSTM in SemEval-2017 Task 8 Subtask A.

The original branchLSTM project address: https://github.com/kochkinaelena/branchLSTM.

In this project, we conduct a non-exhaustive 5-fold cross validation to the original extended PHEME dataset in SemEval-2017 Task 8.

We change the "eval_train_model()" function on predict.py file, use regular expression package to extract the maximum branch length from saved npy file, to make it able to train on other dataset with different maximum branch length.

To apply branchLSTM on other dataset with different scale of conversations, you can change the dataset loading part befor using "preprocessing()" method in preprocessing.py.

Read README.md in downloaded_data/ to download depend files.

To run the experiment pipeline, use "sh run_branchLSTM_pipeline.sh"
