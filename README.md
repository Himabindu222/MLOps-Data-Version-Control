# MLOps-Data-Version-Control
DataVersionControl

1. Install python
   
2. mkdir data
 
3. run the file dataset.py  using the command python3 dataset.py
   
   This creates a file named sample_data.csv under data directory.
   
4. install dvc
   
   pip install dvc
   
5. Run below command which creates  .dvcignore, .dvc.
   
   dvc init
   
6. Run the below command to track the file with DVC.
   
   dvc add data/sampl_data.csv
   
7. Store the data file remotely in s3
   
  a. create s3 bucket

  b. dvc remote add -d data s3://<s3 bucket name>/
  
  c. aws configure
  
  d. dvc commit
  
  e. python3 -m pip install dvc_s3
  
  f. dvc push
  
8. Store .dvc file in Github repo

  a. git add data/sample_data.csv

  b. git commit -am "first version"
  
  c. git add .dvc
  
  d. git commit -am " configuration file "
  
  e. git push origin main





