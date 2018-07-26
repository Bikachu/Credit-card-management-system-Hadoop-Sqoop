# Credit-card-management-system-Hadoop-Sqoop
This project use Sqoop to  import data from MySQL(Linux) to HDFS

-----------------------------------------
1. The MySQL database:  JDBC is in linux and contains THREE tables:

             CDW_SAPP_BRANCH;
             CDW_SAPP_CUSTOMER;
             CDW_SAPP_CREDITCARD;
 The database source file is not provided due to privacy.
 
 According to the mapping document, a forth  " table "  CDW_SAPP_TIME is should be created.
 Sqoop import the data for buidling the CDW_SAPP_TIME to HDFS.
 
 2. Sqoop import the data from MYSQL to HDFS and stores the data as textfiles.
 
 3. The directories shouldn't be created before running the query cause the execution of sqoop will automatic create directories.
 
 4. These queries can also be saved as sqoop jobs:
 
 
 5. Sqoop job commands:
 
 
                   list sqoop job: 
                   sqoop job --list -meta-connect jdbc:hsqldb:hsql://localhost:16000/sqoop

                   kill sqoop job:
                   sqoop job --kill __ -meta-connect jdbc:hsqldb:hsql://localhost:16000/sqoop
                   
                   run sqoop job
                   sqoop job --meta-connect jdbc:hsqldb:hsql://localhost:16000/sqoop --exec BranchJob
  
  If the sqoop job is created and running on sqoop metastore, make sure the sqoop metastore is running when the sqoop job is executing.
       
