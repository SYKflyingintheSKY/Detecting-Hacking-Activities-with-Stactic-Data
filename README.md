# Aim
Deploying machine learning models which can integrate with Spark cluster to process large amounts of stactic data and detect any potential hacks

# Information on Dataset
Four data files recorded from Linux systems are provided, which captures information relating to the memory activity, and process activity. They are a subset of the Internet of
Things dataset collected by Dr. Nour Moustafa, from IoT devices, Linux systems, Windows systems, and network devices. For more detailed information on the dataset, please refer to the Metadata file (https://ieee-dataport.org/documents/toniot-datasets).

In this project, the memory activity and the process activity data are provided separately, without explicit linkage or computer ID to link up memory and process. For each
data, there is a binary label and a multi-class label, one for indicating whether the activity is an attack or not, and the other for indicating which kind of attack the activity is under.

# Package Restrictions
For the data pre-processing and the machine learning processes: use only PySpark SQL / MLlib / ML packages. 
For the data visualisations: use only Matplotlib packages 
Excessive usage of Pandas for data processing is discouraged.
