# Bird Species Identification using Neural Networks

## Project Title:
Bird Species Identification Using Neural Networks Based on Audio Clips

## Abstract:
This project involves identifying bird species based on their vocalizations using neural networks. We focused on two main objectives:
1. **Binary Classification**: To predict whether a bird call is from an American Crow (Amecro) or a Blue Jay (BlueJay).
2. **Multi-Class Classification**: To classify bird calls into 12 different species, including the American Crow, Barn Swallow, Black-capped Chickadee, and others.
   
The project employs Convolutional Neural Networks (CNNs) for extracting features from spectrograms of bird calls. Performance is evaluated using accuracy, confusion matrices, and loss/accuracy plots. We also applied pruning and ensemble techniques to improve model performance, resulting in an overall successful classification of bird species. These models can be applied to bioacoustic research and wildlife monitoring systems.

## Project Structure:
- **Neural-Networks-Bird-Sound-Classification.ipynb**: This Jupyter notebook contains the complete code for data preprocessing, model development, training, and evaluation.
- **Neural-Networks-Bird-Sound-Classification-Report.pdf**: The final report detailing the analysis, methodologies, results, and conclusions.
- **README.md**: This file, providing an overview and instructions for the project.

## Installation:
Clone the repository using the following:

git clone https://github.com/jananikrishnamurthy17/Neural-Network-Bird-Sound-Classification.git

## Dataset:
The dataset used in this project contains bird calls from 12 species recorded in the Seattle area. Each entry includes a spectrogram representing the sound of a bird call, along with its associated label (bird species).

## Methodology:
1. Data Preprocessing:

Resampling audio clips to 22050 Hz.
Segmenting clips into 2-second windows containing loud bird calls.
Generating spectrograms from these clips to use as input features for the neural network.

2. Model Development:

**Binary Classification Model**: Predicts whether a bird call is from an American Crow or Blue Jay.
**Multi-Class Classification Model**: Classifies calls into one of the 12 bird species.

3. Model Evaluation:
   Convolutional Neural Networks (CNNs) were used to extract features from the spectrograms. Various model architectures and configurations were tested, including ensemble methods like bagging and boosting.

**Metrics Used**: Accuracy, Confusion Matrix, and Loss/Accuracy Plots.
**Ensemble Techniques**: Pruning and cross-validation were applied to enhance model performance.

## Results:

**Binary Classification**: Achieved an accuracy of 96% after training the model.
**Multi-Class Classification**: Achieved an accuracy of 72.38% on the test set.
**External Data Testing**: The model was tested with external audio clips, where all three samples were predicted to be Dark-eyed Junco calls, demonstrating some limitations of the model with unseen data.

## Conclusion:
This project demonstrates the application of neural networks for identifying bird species based on their vocalizations. The models achieved strong performance on the training dataset, although challenges arose when classifying external audio clips. The findings could have practical applications in bioacoustic monitoring and wildlife conservation efforts.
