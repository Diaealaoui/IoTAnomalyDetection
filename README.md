This project implements a hybrid machine learning model to detect anomalies in sensor data collected from IoT devices. It uses an Autoencoder for feature extraction and a Decision Tree Classifier for classification.

Dataset Description
The data used in this project was recorded from a DHT11 sensor connected to a TinyML Kit. The dataset includes temperature readings (in °C) and humidity readings (in %). The collected data was preprocessed and fed into the model to identify abnormal readings that may indicate sensor faults or environmental anomalies.

Here you can find the Dataset recorded from our project:  https://www.kaggle.com/datasets/diaealaouisoulimani/iot-t-sensor-dataset-for-anomaly-detection/data 

Model Architecture
The model combines two components. First, an Autoencoder learns a compressed representation of normal sensor behavior. Then, a Decision Tree Classifier uses the encoded features to classify each data point as either normal or anomalous. This approach enables lightweight and efficient anomaly detection suitable for resource-constrained environments.

Project Structure
The main code is provided in the notebook file anomaly_detection_in_iot_devices.ipynb, which includes all steps such as data loading, preprocessing, model training, evaluation, and visualization.

Dependencies
This project requires Python 3.x and the following libraries: pandas, numpy, scikit-learn, and TensorFlow/Keras. These can be installed using pip:


pip install pandas numpy scikit-learn tensorflow

How to Run
Download or clone the project. Place the dataset file (e.g., clean_unlabeled_dataset.csv) in the same directory as the notebook. Open the notebook in Jupyter or Google Colab and run all cells sequentially to execute the pipeline.

Evaluation
Model performance is evaluated using standard classification metrics such as precision, recall, and F1-score. Additional visualizations are used to analyze the reconstruction error and understand the model’s accuracy in identifying anomalies.

Note
This project is based on real-world data collected from a physical sensor setup. The DHT11 sensor was used to record temperature and humidity readings, which were then processed by a machine learning model implemented on an ML development kit.

This project was fully developed by AUI students (Abdellahi Beddi, Diae Alaoui Soulaimani and Malak Errifai) for Machine Learning course supervised by Dr. Yousra Chtouki

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
