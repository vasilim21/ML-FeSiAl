# Machine learning assisted optimization of soft magnetic properties in ternary Fe-Si-Al alloys.
The repository contains supplementary material for the paper. Here is the content list:
1) Dataset_raw.csv. Initial dataset used in this work.
2) Dataset_raw_statistic.html. Detailed statistics of the initial dataset
3) Dataset_preprocessed.csv. Dataset after some data transformations and cleaning.
4) Dataset_preprocessed_statistic.html. Detailed statistics of the preprocessed dataset.
5) Five ML models (MLP algorithm) for the prediction of individual properties in FeSiAl alloys. Before training the models, the independent variables (composition) were standardized, therefore, to use the trained models, first it is necessary to use Scaler, which are individual for each property (except for the initial and maximal permeability) since the number of data points, and therefore the compositions used for training, differ depending on the property. The composition must be specified in the format Si-Al-Fe. 
    - Polarization.pkl; Scaler_Polarization.pkl. ML model and scaler for the prediction of saturation magnetic polarization in T.
    - IP.pkl; Scaler_permeability.pkl. ML model and scaler for the prediction of initial relative magnetic permeability (logarithm). 
    - MP.pkl; Scaler_permeability.pkl. ML model and scaler for the prediction of maximal total relative permeability (logarithm).
    - Coercivity.pkl; Scaler_Coercivity.pkl. ML model and scaler for the prediction of coercivity in A/m.
    - Resistivity.pkl; Scaler_Resistivity.pkl. ML model and scaler for the prediction of specific electrical resistivity in µΩ•cm.
6) Dataset with predicted properties for 22800 compositions FeSiAl with Si and Al content up to 15 wt.% and step 0.1 %. 
