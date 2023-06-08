This repository contains the following structure high level:

    .
    ├── src                    
    │   ├── data_extraction        # API project
    │   ├── ├── src
    │   ├── ├── ├── api
    │   ├── ├── ├── config
    │   ├── ├── ├── helpers
    │   ├── ├── ├── logs
    │   ├── ├── ├── transfer            # (for transfering data from API to S3)
    │   ├── ├── ├── app.py              # (for lambda execution)
    │   ├── ├── ├── main.py             # (for local execution)
    │   ├── ├──  Dockerfile             # (for lambda execution using ECR) 
    │   ├── ├──  requirements.txt   
    │   ├── dbt_deploy             # Dbt Project
    │   ├── ├── dbt_project             # (with bronze, silver and gold models)
    │   └──  ...                 
    └── ...
