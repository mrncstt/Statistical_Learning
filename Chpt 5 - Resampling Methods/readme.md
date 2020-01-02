
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
