# FLAMES2Graph: An Interpretable Federated Multivariate Time Series Classification Framework

## Additional qualitative examples of the extracted subsequences and evolution graphs

In the examples below, we demonstrate additional cases by taking a closer look at the interpretability capacity and the effectiveness of our proposed FLAMES2Graph framework for the ECG (2-dimensional) and UWave(3-dimensional) datasets.

## ECG dataset
![ECG](https://user-images.githubusercontent.com/85762194/231487225-e5295a48-c872-42b6-a5db-a20c80ea7403.png)

For high resolution you can download the pdf file 
[ECG.pdf](https://github.com/anonymousger/FLAMES2Graph-Additional-examples/files/11212214/ECG.pdf)


## UWave dataset
Our framework is tested on two samples from the UWave dataset, as shown in this example. The first sample (a) includes three representative patterns (nodes 17, 11, and 18) that were learned from the network, while the second sample (b) consists of representative MHAP nodes 22, 4, and 11. The graph represents the relationship between these nodes based on their temporal occurrence order in (c). Notably, node 11 is present in both samples, but its temporal order is different in the two classes. Our graph representation plays a crucial role in identifying the representative patterns and their chronological order, aiding the classifier in making a specific decision.

