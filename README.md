# Identifying Stellar Cluster Membership
This project applies machine learning to classify stars in noisy, real-world data, showing how to extract reliable signals and evaluate model performance in a complex classification problem.

## **Overview**
This project applies supervised machine learning techniques to identify stellar cluster members of Praesepe Cluster using observational data. The goal is to distinguish true cluster members from field stars by leveraging astrometric and photometric features, which often contain noise and measurement uncertainty.

This problem is analogous to real-world classification tasks where signal must be extracted from overlapping, noisy data distributions.

## **Key Questions**
- Can we accurately distinguish cluster members from field stars using observational data?
- Which features (e.g., parallax, proper motion, photometry) are most informative for classification?
- How well does the model generalize, and where does it make mistakes (false positives vs. false negatives)?

## **Methodology**
- Data Preparation
    - Compiled stellar deta include positional, kinematic, and photometric features
    - Cleaned and filtered data to remove incomplete or low-quality features
- Feature Engineering
- Trained a Random Forest Classifier to model and distinguish members from non-members
- Assessed performance using classification accuracu and confusion matrix
- Visualized results in parameter space

## **Results**
- The RF model successfully identified cluster members with high accuracy, correcly classifiying the majority of known members and non-members
- Feature importance analysis showed that parallax and proper motion were the strongest predictors, aligning with physical expectations.
- The model’s predictions were consistent with literature values, increasing confidence in its reliability
  
## **Repository Structure**
`data\` # Input datasets (field stars and members of Praesepe Cluster)

`notebooks\` # Jupyter notebooks for searching for members and applying random forest classifier 
