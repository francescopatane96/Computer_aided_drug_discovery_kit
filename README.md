# Computer_aided_drug_discovery_kit

This pipeline provides a way to perform pharmaceutical compounds virtual screening using similarity-based analysis, ligand-based and structure-based techniques.The pipeline contains a collections of modules to perform a variety of analysis.

ML_1: Use of ChEMBL database to extract data (IC50, canonical smiles) from it for compounds associated with a target of interest. Data sets can be used for many cheminformatics tasks, eg. similarity search and clustering or machine learning. 

In this notebook you will find compounds which were tested against a specific target and filtering available bioactivity data. Then, for every single compound, lipinki's descriptors are calculated, together with Padel's decriptors.

ML_2: 

ML_3: Unwanted substructures filtering and substructure statistics.

ML_4: Similarity-based virtual screening.

ML_5: 

ML_6: 

ML_7: Machine learning generation module using Padel descriptors as features. Data extracted from Chembl are used to train a RandomForest classifier to determine the correct class of origin of new unseen compounds (pharmaceutical screening). Data are previous split into 3 classes (low, medium, high) of bioactivity level. RandomForest model is then validate using a ratio 20:80 test set and metrics are evaluate using cross-validation methods. The module allows you to change ML parameters to obtain a good predictor for your target of interest. Metrics and statistics (confusion matrix, eg.) can be obtain.

ML_7.1: prediction module. the joblib object generated in the previous model is used to predict the class of every new compound.
