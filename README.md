# Internet Firewall Data Classification

## Overview
This project applies several machine learning algorithms to classify internet firewall data into different action categories. The dataset used for this classification task comes from the [Internet Firewall Data](https://archive.ics.uci.edu/dataset/542/internet+firewall+data) repository.

### Objective
The goal of this project is to implement and evaluate commonly used machine learning algorithms on a multi-class classification problem. By analyzing network traffic attributes, we aim to distinguish between different firewall actions, enhancing network security decision-making.

## Machine Learning Algorithms Implemented
This project explores and implements the following machine learning techniques:

1. **Principal Component Analysis (PCA)** - Used for dimensionality reduction.
2. **Least Squares Classification** - A simple linear classification approach.
3. **Logistic Regression** - A probabilistic model for binary and multi-class classification.
4. **K-Nearest Neighbors (KNN)** - A distance-based classification method.
5. **Naïve Bayes** - A probabilistic classifier based on Bayes' theorem.
6. **Multilayer Perceptron (MLP)** - A feedforward neural network model.
7. **Support Vector Machines (SVM)** - A powerful classification method using hyperplanes.
8. **K-Means** - A clustering algorithm to identify patterns in the data.

Each algorithm is tested on the firewall dataset to evaluate its performance in classifying network traffic behavior.

## Dataset Description
The dataset consists of 12 features, with the **'Action'** feature representing the target variable. Below is the description of each feature:

| Variable Name          | Description                            |
|------------------------|----------------------------------------|
| Source Port           | Sender's initiating port.             |
| Destination Port      | Receiver's target port.               |
| NAT Source Port       | Sender's port after NAT.              |
| NAT Destination Port  | Receiver's port after NAT.            |
| Bytes                | Packet size in bytes.                 |
| Bytes Sent           | Bytes sent by the sender.             |
| Bytes Received       | Bytes received by the receiver.       |
| Packets              | Total packets transmitted.            |
| Elapsed Time (sec)   | Duration of communication.            |
| pkts_sent           | Packets sent by the sender.           |
| pkts_received       | Packets received by the receiver.     |
| Action              | Class label (e.g., allow, block, etc.).|

### Classification Task
The goal is to classify each network traffic observation into one of the following four classes:

- **allow**
- **deny**
- **drop**
- **reset-both**

Each record belongs to only one of these classes. The classification models are evaluated based on their accuracy and ability to generalize to unseen data.
