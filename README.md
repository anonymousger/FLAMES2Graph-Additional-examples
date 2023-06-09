# FLAMES2Graph: An Interpretable Federated Multivariate Time Series Classification Framework

## Additional qualitative examples of the extracted subsequences and evolution graphs

In the following examples, we demonstrate additional cases by taking a closer look at the interpretability and effectiveness of our proposed FLAMES2Graph framework for the ECG (2-dimensional) and UWave (3-dimensional) datasets.

## ECG dataset

![Capture](https://user-images.githubusercontent.com/85762194/231527935-e88d8072-b305-42c5-8eac-bd30f5c04864.PNG)

This example demonstrates the MHAP evolution graph for ECG data and the temporal transitions for a Class 1 data set sample. The framework identifies the important subsequences of the multivariate time series data and represents the temporal transition through the MHAP evolution graph. Figure (a) shows the three MHAPs extracted from the class 1 sample that serve as nodes in the graph shown in (b). The transitions between the nodes show the order of occurrence of the MHAPs in the input data. To understand the decision of the network in classifying time series, our framework relies on the important subsequences of the input data (MHAPs) and their temporal order, which is crucial. For instance, when interpreting ECG data, a physician needs to examine the data in a specific temporal sequence to determine whether the patient's ECG recording is normal or has pathological problems.

## UWave dataset

![Capture1](https://user-images.githubusercontent.com/85762194/231794593-57c17149-7a70-428a-a06d-8325b69dfbb7.PNG)

Our framework is tested on two samples from the UWave dataset, as shown in this example. The first sample (a) includes three representative patterns (nodes 1, 2, and 3) that were learned from the network, while the second sample (b) consists of representative MHAP nodes 4, 5, and 2. The graph represents the relationship between these nodes based on their temporal occurrence order in (c). Notably, node 2 is present in both samples, but its temporal order is different in the two classes. Our graph representation plays a crucial role in identifying the representative patterns and their chronological order, aiding the classifier in making a specific decision.

As we analyze sample (a), it becomes apparent that the first output class label is activated in both the x and y-axis signals of the UWave dataset. This label corresponds to a gesture pattern that starts at a specific point, moves upwards, towards the left, and finally downwards, as shown by the 'output label shape' in (a). Although this information provides insight into the pattern recognition process, a domain knowledge expert can provide a more nuanced interpretation of the outputs. Our framework is designed to help the user visualize the significant input subsequences that contribute to a specific decision, thereby facilitating precise interpretation by domain experts.
