# Federated Learning with Chest X-Ray Images

This project demonstrates the application of federated learning using a ResNet-34 model to classify chest X-ray images into various conditions. The implementation leverages PyTorch and torchvision for model building and training, and is designed to run on Kaggle's notebook environment.

## Project Overview

### Objective
The objective of this project is to utilize federated learning for training a neural network model on chest X-ray images without centralizing the data. Federated learning allows the model to be trained across multiple devices (clients) that hold local datasets, ensuring data privacy.

### Dataset
The dataset used in this project is the NIH Chest X-ray dataset, which contains over 100,000 chest X-ray images with 14 different thoracic disease labels. The data is preprocessed and loaded from the Kaggle input directory.


## working of the Project

1. **Load the Data**:
    - Walk through the input directory to list all files and locate the dataset files.

2. **Preprocess Data**:
    - Read the CSV file containing metadata and preview the data to understand its structure.

3. **Display Sample Image**:
    - Define functions to load and display images to verify data integrity.

4. **Define Dataset and DataLoader**:
    - Create a custom dataset class to handle image transformations and label encoding.
    - Implement a DataLoader for batching and shuffling the data during training.

5. **Define Federated Network and Client Classes**:
    - Build the federated learning network based on ResNet-34.
    - Create a client class to handle local training and parameter updates.

6. **Set Up Clients and Start Training**:
    - Split the dataset among multiple clients.
    - Initialize the global model and start the federated training process across defined rounds.

7. **Visualize Training History**:
    - Plot training and validation losses over the training rounds to monitor model performance.
    - (added screenshot from round 8 to round 10)
   
      ![image](https://github.com/Arjun-08/Federated-learning-over-IOMT/assets/88790572/d4c49d27-e52c-446d-957d-203314e31a61)


## Results

The model is trained using federated learning, and the performance is evaluated based on training and validation losses. The training history is visualized to show the progression of the training process.

![image](https://github.com/Arjun-08/Federated-learning-over-IOMT/assets/88790572/df0870e5-430c-4083-90fb-80befeabcd5f)


## Conclusion

This project showcases the implementation of federated learning using a deep neural network for medical image classification. The approach ensures data privacy and can be extended to other applications requiring decentralized learning.

## Contact

If you have any questions or suggestions, please feel free to reach out to me at [nvarjunmani07@gmail.com](mailto:nvarjunmani07@gmail.com).

