# FaultNet: A Deep-Learning Framework for Unsupervised Time-Series Analysis and Anomaly Detection

Every day, vast amounts of unlabeled time-series data are collected across the globe, particularly status of health (SOH) data for equipment system monitoring and predictive maintenance. Unfortuantely, because this data is unlabeled, traditional supervised machine learning techniques are inapplicable, and unsupervised techniques, such as clustering, are demanded. Time-series clustering is an important and growing field, but there are many inherent challenges, such as missing data and complex time dependancies. In this work, we explore the unique challenges of time-series clustering, and present FaultNet, a data-driven framework for the rapid analysis and classification of unlabeled time-series data.

### _Task_:
Our task is two-fold:

1) Implement the Siamese-shift Encoder, a neural-network embedding function for transforming unlabeled time-series data onto a low-dimensional embedding space, where the embeddings are robust to temporal shifts and gaps, but sensitive to all other temporal anomalies.

2) Implement FaultNet, a framework for the rapid analysis of the time-series data, based on shift-encoded embeddings. FaultNet includes tools for both manual visual exploration, and automated anomaly detection.


### _Dataset_:
To train and test the network, we make use of a common time-series SOH streams: Battery Voltage. The data used comes from a Status of Health Server, which contains just over 2 years of data across 148 seperate equipment sites. These sites all operate at a nominal battery voltage of either 12 or 24V. Additionally, the power is supplied to the batteries by either Commercial Power or Solar Power.

### _Overview_:

In the remainder of this notebook, we will proceed as follows:

* STEP 1: EXPLORE THE DATASET

* STEP 2: DEFINE AND TRAIN THE ENCODER

* STEP 3: ANALYZE THE ENCODINGS
