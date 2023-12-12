1.	Problem Formulation:
Processing Time:
Traditional analytics struggle in processing air quality data efficiently due to its volume and complexity. The proposed problem aims to reduce the processing time for air quality data through the implementation of big data analytics.[1]
Scalability:
Conventional analytics often overlook external factors such as meteorological conditions and traffic patterns, which influence air quality. It is not easy to adapt to the analysis.

2.	Conventional Techniques:
In conventional data analytics, the chosen approach relies on traditional tools and frameworks, primarily utilizing the Pandas library in Python. The workflow involves loading data into a Pandas DataFrame, which provides data analysis environment. The elapsed time of each step is computed to be compared with Big Data Analytic techniques. 
Here's an overview of the conventional techniques in the provided code snippets:

3.	Big Data Analytics Techniques:
Spark, a powerful big data analytics processing engine will be applied to the same air quality dataset as a contrast to conventional big data analytics techniques.

Processing Time for different stages of data analytics processes, both for Conventional Techniques and Big Data Analytics Techniques. The percentages represent the proportion of time each stage takes in the total process. 

![image](https://github.com/SeanLing94/placeholder/assets/143430094/200e7935-8760-4e41-bb5b-f70c34a015fd)

Key Takeaway:
•	Big Data Analytic Techniques are 8 times slower than conventional techniques.
•	Conventional techniques took longer time in loading the data while big data analytics in Data Aggregation. 
•	Conventional techniques took shorter time in data processing while big data analytics in data transformation.
•	Big data analytic techniques have very similar processing time for small/large scale data. (0.2231s vs 0.2300s)
•	Processing time for large-scale data is twice the small-scale in conventional techniques. (0.0003s vs 0.0006s)

5.	Discussion & Explanation of Comparison:
Big Data Analytic Techniques are 8 times slower.
•	Spark operates data across multiple nodes in a cluster. The overhead of managing this distributed environment, including data distribution, communication, and coordination among nodes, can contribute to increased processing time compared to a single-node conventional approach.
•	The chosen data volume is not substantial enough to fully utilize the parallelism.
•	Spark requires initialization and setup time to distribute tasks across the cluster and set up the parallel processing.[3] Conventional techniques may have a faster startup time since they don't involve the same level of coordination and resource allocation.

Conventional techniques took longer time in loading the data, big data analytics in Data Aggregation. 
•	Conventional techniques, especially those implemented in single-node environments using tools like pandas in Python, typically load and process data sequentially on a single machine.
•	Spark leverage distributed parallel processing across a cluster of machines, dividing the data and computation tasks among multiple nodes.

Conventional techniques took shorter time in data processing while big data analytics in data transformation.
•	Panda in python can contribute to faster data processing for tasks like filtering, sorting, and basic transformations in conventional techniques.
•	Data Transformation in big data analytics can handle complex transformations and include the creation of new features through pipelines easily.
 
Scalability test
•	100% incremental from small to large scale in data processing time which in directly proportion observed in conventional techniques. 
•	Conventional techniques often load the entire dataset into memory for processing. As the dataset size increases, the available memory may become a bottleneck.
•	Conventional techniques typically operate on a single machine, which may have limitations in terms of processing power and memory compared to a distributed environment.
•	3% incremental from small to large scale in data processing time in big data techniques.
•	The techniques are designed to scale efficiently with data size.
•	Big data analytics frameworks often leverage distributed processing, enabling parallel execution across multiple nodes or clusters.
•	Spark uses optimized storage formats and retrieval mechanisms.
