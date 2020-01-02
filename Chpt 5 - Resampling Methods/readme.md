
## 5.1. Cross-Validation and Bootstrap


![](https://i.imgur.com/xNkDSgR.png)



Q1 When we fit a model to data, which is typically larger?

- **Test Error**
- Training Error


Q2 What are reasons why test error could be LESS than training error?

- **By chance, the test set has easier cases than the training set.**
- The model is highly complex, so training error systematically overestimates test error
- The model is not very complex, so training error systematically overestimates test error

## 5.2 K-fold Cross-Validation
![](https://i.imgur.com/gAVZa4I.png)

### In each stage, one part gets to play the role validation set. The other four parts are the training set.


Q1 Suppose we want to use cross-validation to estimate the error of the following procedure:

Step 1: Find the k variables most correlated with y

Step 2: Fit a linear regression using those variables as predictors

We will estimate the error for each k from 1 to p, and then choose the best k.

True or false: a correct cross-validation procedure will possibly choose a different set of k variables for every fold.

- **TRUE**
- FALSE


## 5.3 Cross-Validation: the wrong and right way


Q1 Suppose that we perform forward stepwise regression and use cross-validation to choose the best model size.

Using the full data set to choose the sequence of models is the WRONG way to do cross-validation (we need to redo the model selection step within each training fold). If we do cross-validation the WRONG way, which of the following is true?


- **The selected model will probably be too complex**
- The selected model will probably be too simple
