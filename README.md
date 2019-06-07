# Machine Predictive Maintenance (PdM)

Predictive maintenance techniques are employed to determine the condition of in-service equipment in order to estimate when maintenance should be performed. The main promise of predictive maintenance is to allow convenient scheduling of corrective maintenance, and to prevent unexpected equipment failures.

In this project I aim to apply predictive maintenance techniques over 100MB of historical data from twenty of the units of a company that failed in the field. The shortest-lived units failed after a few days; the longest-lived units failed after several years. Typical lifetimes are on the order of a year.

The company has a remote monitoring system for the motors in each unit, which collects information about the motor (rotation speed, voltage, current) as well as two temperature probes (one on the motor and one at the inlet). My objective is to see if there is a similarity in information of the units who had longest lives or shortest lives. The idea is to find a pattern which can help us to determine whether a unit will fail soon or not.

Also, the company has thirty active units working in the field from the past month. My another objective would be to predict which units will fail soon from the available information of previously failed units.

## Libraries Used: 
- Keras
- fastdtw
- glob
- scipy
- sklearn

## Steps:
- Introduction
- Importing Libraries
- Importing Data
- Data Cleaning
- Data Imputation
- Exploratory Data Analysis
- Clustering
  - Dynamic Time Warping
  - Hierarchical Clustering
- Classification
  - Data Preprocessing
  - LSTM Model
  - Machine Failure Probabilities
- Conclusion
