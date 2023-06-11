# Job Salary Prediction
This project aims to predict the salaries of job postings based on the provided training dataset. The project is divided into several stages: preprocessing the data, training the model, using random optimization to tune the hyperparameters, active learning to add unlabelled data, and evaluation using K-fold and validation dataset.



## Authors

- [@August Xu](https://github.com/AugustRushG)


## How to run locally
1. Ensure you have python 3.9 or above to run locally 
```
Python --version
```
2. Install the required libraries.

```
$ pip install sentence-transformers
```

3. Then Just replace all datasets path to where you located.
```
raw_train_data = pd.read_csv('train.csv')
raw_test_data = pd.read_csv('test.csv')
raw_valid_data = pd.read_csv('valid.csv')
```
4. Run the code
## How to run on Colab
1. Open the provided Jupyter notebook in Google Colab.

2. Replace all datasets path to where you located.

3. Run the code.

## Sections
### Pre-processing Data
The first step is to preprocess the data using the sentence transformer and scalar. This will convert the data into high-dimensional vectors, which will be used for model training.
### Training Models
Several models will be selected to train on the embedded data. The hyperparameters will be tuned using random optimization.
### Active learning
Active learning will be used to add unlabelled data to the model. This will be done through a loop, and the batch size of each round can be changed. However, this will impact the speed of the process.
### Evalution
The evaluation will be done using K-fold and validation dataset. The accuracies will be used to evaluate the model, but other metrics can also be used.
### Exporting Results
Finally, the test result will be exported using the model chosen.