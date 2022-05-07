## Data and Machine Learning Projects

### Neural Network from scratch    &emsp; [github](https://github.com/td-iceman/Tarandeep-Projects/blob/main/Neural%20Network%20from%20scratch/NN_from_scratch.ipynb)

Hands-on ML project for understanding neural network inner workings and learning to implement in python. Used this to test the *hello world* problem of neural networks classification, recognizing hand-written digits from the MNIST database. Following are the highlights from the project:

- Implemented *Layer* class in python for *activation* and *backpropogation*.
- Incorporated *Adam optimizer*, *sigmoid* activation function, *mean square error* cost function and *mini-batch* training method.
- 15 neuron hidden layer network classified 90 % digits correctly (tensorflow: 94 %)

![mnist](/Tarandeep-Projects/images/MNIST_digit.jpg)

<br />

### Heart Disease prediction - Kaggle dataset     &emsp; [github](https://github.com/td-iceman/Tarandeep-Projects/tree/main/Heart%20Disease%20Prediction)

Used open dataset for heart patients from Kaggle datasets and trained various decision tree-based classification models. Also used SHAP model explainer to the best model to develop data insights for prediction. Project summary:

- Cleaned and explored data, creating dummy attributes. &emsp;[code](https://github.com/td-iceman/Tarandeep-Projects/blob/main/Heart%20Disease%20Prediction/Heart_Disease_data_processing.ipynb)
- Applied *Decision Tree* and *Random Forest* models for prediction. &emsp;[code](https://github.com/td-iceman/Tarandeep-Projects/blob/main/Heart%20Disease%20Prediction/2_Heart_Disease_decision_tree_random_forest.ipynb)
- Applied *Gradient Boost* model for prediction. &emsp;[code](https://github.com/td-iceman/Tarandeep-Projects/blob/main/Heart%20Disease%20Prediction/3_Heart_Disease_gradient_boost.ipynb)
- Applied *XGBoost* model for prediction and *SHAP* for model explanation. &emsp;[code]()

Model performance comparison:
 Model | Train score | Test score | CV score | CV std 
 --- | --- | --- | --- | --- 
 **Decision Tree** | 96 % | 82.6 % | 82.5 % | 7.9 % 
 **Random Forest (tuned)** | 94.4 % | 85.7 % | 86.8 % | 6.5 % 
 **Gradient Boost (tuned)** | 100 % | 85.7 % | 87.4 % | 6.1 % 
 **XGBoost (optimized)** | 99.2 % | 88 % | 88 % | 6.8 % 

Highlights of *XGBoost* model explanation and analysis:
- Found out that attritbute data imbalance (sex: *female* and target outcome within that set) was wrongly employed by model as an important prediction feature.
- Observed candidates for feature selection/reduction for model simplification.
- Obesrved few features and trends of their impact on outcome. 

![shap](/Tarandeep-Projects/images/shap.jpg)
