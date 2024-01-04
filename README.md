# NIDS_Project
This project utilizes machine learning to analyze PCAPs or CSVs of captured packet data and train a model to identify anomalies on web traffic

-----------------------------------------------------------First Commit---------------------------------------------------------

The first commit of the project trained a decision tree model utilizing the scikit-learn python library with the the CICIDS2017 dataset from Kaggle (https://www.kaggle.com/datasets/cicdataset/cicids2017)
Simplifications were made to data set using the 'Label' column which had multiple values like: Brute Force FTP, Brute Force SSH, DoS, Heartbleed, Web Attack, Infiltration, Botnet and DDoS   
A new column was created called 'ATTACK/BENIGN' which was based off of the 'Label' column values assigning either ATTACK or BENIGN.
Since this was my first time training a model I wanted to simplify the potential values for the model to predict.
The model trained has a preditive accuracy score of 99.98% 

NOTE: The PCAP aggregator part of the function is not fully finished, I thought it would be interesting to build something that could aggregate PCAP files if I wanted to implement something like Pyshark to capture live packet data. So far that part of the function is just a shell. 
