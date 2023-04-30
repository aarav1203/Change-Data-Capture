# Problem Statement
Create Automated Pipeline that capture the data change(means when first time any new data come  then store completely but if any update happen in the previous storing data then it will only change that data not again store completely) from Relatational Database (Source) and store into some cloud storage(Destination Point).

## Techstack Used
1. AWS
2. MYSQL 
3. Python

## Infrastructure Used
1. AWS Glue
2. S3 Bucket
3. AWS RDS
4. DMS
5. Lambda

## Project Architecture
![alt text](https://raw.githubusercontent.com/aarav1203/Change-Data-Capture/main/Aws%20project.png)

### Folder Structure
Prefer to make separate bucket for input and output operation
Input :- Bucket/Folder/File
Output:- Bucket/Folder/File



## Conclusion
Any changes will made in database ,this will automatically detect and lambda will invoked glue job and after that load into s3 bucket
