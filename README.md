# ETL-Log-Processing-using-Airflow

This repository contains Python code to define an Airflow DAG for processing server access logs. The DAG performs the following tasks:

Extract: Extracts timestamp and visitor ID fields from the access log file.
Transform: Capitalizes the visitor ID in the extracted data.
Load: Compresses the transformed data into a tar archive.

Files Included:
ETL_Server_Access_Log_Processing.py: Python code defining the Airflow DAG.
ETL_Server_Access_Log_Processing.sh: Shell script for performing data extraction, transformation, and loading.

Requirements:
Python 3 with airflow library installed.

How to Use:
Copy Files: Copy both Python and shell script files to your Airflow DAGs directory:

Bash
cp ETL_Server_Access_Log_Processing.py $AIRFLOW_HOME/dags
cp ETL_Server_Access_Log_Processing.sh $AIRFLOW_HOME/dags
Use code with caution.
Set File Permissions: Ensure the shell script is executable:

Bash
cd $AIRFLOW_HOME/dags
chmod +x ETL_Server_Access_Log_Processing.sh
Use code with caution.
Schedule the DAG: Use the Airflow UI or command line to schedule the DAG.

Note: This example assumes the access log file resides at /home/project/airflow/dags/web-server-access-log.txt. Update the file path in the shell script if needed.

Contributing:
Feel free to fork this repository and submit pull requests with improvements or modifications.

License:
This project is licensed under the terms of the MIT License: https://opensource.org/licenses/MIT.
