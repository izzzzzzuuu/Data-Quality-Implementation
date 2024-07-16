# Data-Quality-Implementation

![image](https://github.com/izzzzzzuuu/Data-Quality-Implementation/assets/46993601/63030f2f-831d-4812-a7ad-c60eff76d354)

## Data Used

**Data** - Hospital dataset over 5 million rows and consist of 5 columns .

**Data Cleaning & Data quality implementation** - Jupyter notebook (Python)

**Data Visualization** - PowerBI

## Aim
> Applying databricks fundamentals such as Medallion architecture (Raw layer/Bronze layer -> Silver layer -> Gold layer) using open source web application 
1. To access the dataset located in Microsoft Azure container
2. Convert the raw file to parquet file format and uploaded it into Azure container, Bronze folder
3. Access via bronze folder to start processing the dataset
4. Upload the processed dataset into Azure container, Silver folder

- Must not delete any data, except after being processed thoroughly within the 5 data quality aspect
- The invalid data, must be modified/fix to ensure it is valid, hence they are split into rejected dataset and accepted dataset.
- After the rejected dataset has been modified, it is merged back to the accepted dataset as a complete and whole dataset 
## Initial issues with dataset

1. Dataset has multiple duplicate values
2. Column name and column email is inaccurate
3. There are issues of consistency in email and its top level domain
4. There are data that is invalid due to age requirements and possesion of title, hence the validity is doubtful
5. Data quality of the dataset is poor, notably in validity, accuracy, and consistency aspects

## 5 data quality aspects workflows
1. Completeness
2. Accuracy
3. Consistency
4. Validity
5. Uniqueness

## Results after processing data
Data quality of the dataset improve significantly, specifically in accuracy, consistency, and validity of the dataset

## Limitations
1. Does not sure the gender of person only based on their name
2. Unsure whether the format for email column is varied from people with title or with no title
3. Unsure whether the same name belongs to the same person or different person, although they have the same values across rows but only with different ID, (temporary solution: Assumed they are different person **due to lac of information in dataset)
