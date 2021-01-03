# Environment
* Ubuntu 20.04 LTS (Focal Fossa) 
* Python (3.8) 
* Jupyter Notebook 
* Apache Spark (3.0.0) 

# Aim
Deploying machine learning models which can integrate with Spark cluster to process large amounts of stactic data and detect any potential hacks

# Information on Dataset
Four data files recorded from Linux systems are provided, which captures information relating to the memory activity, and process activity. They are a subset of the Internet of
Things dataset collected by Dr. Nour Moustafa, from IoT devices, Linux systems, Windows systems, and network devices. For more detailed information on the dataset, please refer to the Metadata file (https://ieee-dataport.org/documents/toniot-datasets).

In this project, the memory activity and the process activity data are provided separately, without explicit linkage or computer ID to link up memory and process. For each
data, there is a binary label and a multi-class label, one for indicating whether the activity is an attack or not, and the other for indicating which kind of attack the activity is under.

# Package Restrictions
For the data pre-processing and the machine learning processes: use only PySpark SQL / MLlib / ML packages.  <br>
For the data visualisations: use only Matplotlib packages. <br>
Excessive usage of Pandas for data processing is discouraged.

# Points which can be improved
* Task 2.2: Creating a custom Transformer for the column “POLI” so that the types of policy, [“norm”, “btch”, “idle”, “fifo”, “rr”, “0”, “-”], can be mapped to the following numbers, [0, 1, 2, 3, 4, 5, 6] - Creating a custom Transform class inheriting from the PySpark ML Transformer, HasInputCol, HasOutputCol, DefaultParamsReadable, DefaultParamsWritable class, so that it can be included in the ML Pipeline in the next step. The class should allow users to specify the inputCol, outputCol, originalValues, and newValues parameters when initiating the object.

* Task 2.3: 
1) When Discussing on which pipeline model is better for both Process & Memory, key points on metric performance, overfitting issue, interpretability, benefits of using Boosting could have been made.
2) ROC curves under different thresholds for both Process & Memory could have been plotted for checking model performance.

* Task 3: Adding information as follows - The first 7 steps are just about initializing the centroids using kmeans++. The next few steps are what perform the iterations and decide the final cluster centers.
