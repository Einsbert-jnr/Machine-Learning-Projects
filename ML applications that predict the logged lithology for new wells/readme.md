### Description of the problem and task
You are working in a geomodelling team in a company specialized in CCS (Carbon Capture and Storage). You have access to a database of logged boreholes, which are intact and complete and given in the same structured input (training_wells.csv). Your goal is to build ML applications that predict the logged lithology for new wells and impute missing values in incomplete logs (mystery_well.csv).

**The data contains the metadata columns**

WELL: well name

X_LOC: UTM X coordinate

Y_LOC: UTM Y coordinate

Z_LOC: DEPTH

**The data contains the well log curves:**

DEPTH_MD: measured depth

CALI: Caliper

RMED: Medium Resistivity

RDEP: Deep Resistivity

RHOB: Bulk Density

GR: Raw gamma data

NPHI: Neutron Porosity

PEF: Photoelectric Absorption Factor

DRHO: Density Correction

DTC: Sonic (Compressional Slowness)

SP: Spontaneous Log

BS: Bit Size

> *The last column 'lithnames' (for the large well collection) is the interpreted lithology.*

**Task 1**
Use the dataset "mystery_well.csv" to come up with a first estimate, how many different lithologies are present in the borehole. ***Build a clusterer model.***

Defend the choice of data and hyper-parameters
Describe the predicted clusters. Should you divide them further?

> Every single detail is captured in the notebook. The notebook contains a well commented code and also all the analysis and conclusion needed

> The labeled csv file is the final csv file which defines the lithology in the boreholes. The mystery_well csv file is the original dataset used for the training.

> K-Means algorithm was used. This an unsupervised machine learning task. Elbow curve was used to identify the optimal number of clusters. Additional evaluation parameters were used to confirm that the optimal number of clusters were indeed the optimal one.