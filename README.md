# **Alphabet Soup Charity Success Prediction Model**

## **Overview**
This project is designed to predict the success of organizations funded by Alphabet Soup. Using a variety of features, including application type, funding amount requested, and sector of industry, the goal is to create a binary classification model that can determine whether an organization will be successful after receiving funding. This model will help Alphabet Soup make better decisions when selecting organizations for future funding.

## **Project Purpose**
The purpose of this project is to:
- Build a machine learning model that predicts the success of Alphabet Soup-funded organizations based on the features provided in the dataset.
- Help Alphabet Soup identify which organizations have the highest potential for success, allowing them to allocate resources more effectively.

## **Data**
The dataset contains over 34,000 organizations that have received funding from Alphabet Soup in the past. It includes features such as:
- **Application Type**: The type of application the organization submitted.
- **Affiliation**: The sector or industry the organization belongs to.
- **Classification**: Government classification of the organization.
- **Income Amount**: The income classification of the organization.
- **Ask Amount**: The amount of funding requested.
- **Is Successful**: The target variable indicating whether the organization was successful.

### **Dataset URL**:  
[Charity Data](https://static.bc-edx.com/data/dl-1-2/m21/lms/starter/charity_data.csv)

## **Model**
This model uses a **Deep Neural Network** for binary classification. The model was built and optimized using TensorFlow and Keras.

### **Model Architecture**:
1. **Input Layer**: Accepts the feature variables.
2. **Hidden Layers**:
   - First hidden layer with 128 neurons and ReLU activation.
   - Second hidden layer with 64 neurons and ReLU activation.
   - Third hidden layer with 32 neurons and ReLU activation.
3. **Output Layer**: A single neuron with a Sigmoid activation function for binary classification.

### **Optimization**:
Several optimization techniques were used to improve the model:
- **Dropout Layers**: Added to prevent overfitting.
- **Increased Neurons**: More neurons were added to hidden layers to make the model more powerful.
- **Modified Epochs**: The number of epochs was adjusted to 150 to allow more learning time.

## **Results**
After training and optimization, the model achieved an accuracy of **66.12%** on the test data. This result indicates that the model can effectively predict the success of organizations funded by Alphabet Soup, though there are still opportunities for further optimization to improve accuracy beyond **75%**.
