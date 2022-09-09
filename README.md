# Predicting the strength of the concrete using Neural Networks
Determining the strength of the concrete with respect to its ingredients using a regression model built in keras.
The accuracy of the model is evaluated in 4 test cases.

## Description of the dataset
The dataset describes the strength of the concrete for different proportions of its ingredients. The various ingredients that helps to determine the strength of the concrete includes:
<ul>
    <li>Cement</li>
    <li>Blast Furnace Slag</li>
    <li>Fly Ash</li>
    <li>Water</li>
    <li>Superplasticizer</li>
    <li>Coarse Aggregate</li>
    <li>Fine Aggregate</li>
    </ul>
    
## PART A
**---------Building a BASE LINE MODEL------------**
<br>
**Charecteristics of the neural network:**
<ul>
    <li><b>1</b> hidden layer - with <b>10</b> nodes</li>
    <li><b>Activation Function</b>: ReLU </li>
    <li><b>Optimizer used</b>: Adam</li>
    <li><b>Loss Function</b>: Mean Squared Error (MSE)</li>
</ul>

The data is randomly split into test sets (**30%**) and train sets (**70%**) and fed into the **Base Line Model**. The model is trained using **50** epochs. Using the test data the model is evaluated and Mean Sqaured Error (**MSE**) is computed.
<BR>
The baseline model is trained and tested **50 times** each time a different train and test data randomly fed from the dataset, thus computing a set of 50 mean squared errors. Hence the best value of mean squared error is computed and standard deviation is also computed from it.

## PART B
Reporting mean of the mean squared error using normalized version of the data with same base line model.
Then the mean of the MSE of normalized and unnormalized data fed into the base line model is comapred with one another.
<br>
<img width="302" alt="image" src="https://user-images.githubusercontent.com/99457944/189320831-0934a561-2b2a-4401-8d57-ba368a1920e5.png">

## PART C
Reporting mean of the MSE using normalized version of the data by increasing the number of epochs to 100
Then the mean of the MSE of the predictions of base line model is computed by increasing the epochs (100)and comapred with that of case B where it is with 50 epochs.
<br>
<img width="286" alt="image" src="https://user-images.githubusercontent.com/99457944/189321430-4312c93e-8f3d-44ad-8425-b9ddae84137a.png">

## PART D
Here, a new neural network model that performs regression is built. The charecteristics of the new model are bleow:
<ul>
    <li>Number of hidden layers: <b>3</b></li>
    <li>Number of nodes in each of the hidden layer: <b>10</b></li>
    <li>Activation function: <b>ReLU</b></li>
    <li>Rest of the features are same as the <b>Base Line Model</b></li>
    </ul>
Then the mean of the MSE of the normalized data is reported. Also the mean of the MSE when the model has 1 hidden layer and when the model has 3 hidden layer is compared with one another.
<br>
<img width="290" alt="image" src="https://user-images.githubusercontent.com/99457944/189321990-26f75fcb-f125-460b-b2a2-7ab1b5936b60.png">

## Observations
Thus it can be onserved that, the mean of the MSE is reduced and accuracy of the prediction is increased when,
<ol>
<li>the data fed into the model is normalized</li>
<li>the number of epochs is increased </li>
<li>the number of hidden layer in the model is incresed.</li>
</ol>
