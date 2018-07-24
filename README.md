# Credit-card-management-system-Hadoop-Sqoop
This project use Sqoop to  import data from MySQL(Linux) to HDFS

-----------------------------------------
1. The MySQL database:  JDBC is in linux and contains THREE tables:

             CDW_SAPP_BRANCH;
             CDW_SAPP_CUSTOMER;
             CDW_SAPP_CREDITCARD;
 The database source file is not provided due to privacy.
 
 According to the mapping document, a forth  " table "  CDW_SAPP_TIME is created based on the CDW_SAPP_CREDITCARD table.
 
 2. Sqoop import the data from MYSQL to HDFS and stores the data as textfiles.
 
 3. The directories shouldn't be created before running the query cause the execution of sqoop will automatic create directories.
 
 
