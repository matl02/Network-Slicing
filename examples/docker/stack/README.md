# Docker compose
This guide demonstrates usage of ```docker compose``` tool for running multi-container applications on Docker defined using the Compose file format.
the `my-stack.yaml` file is used to define how one or more containers that make up your application are configured. 

1. Execute the command below to build a Docker image called ```myserver```, which encompasses all necessary packages to run the `server.py` file:

    ```
    docker build -t myserver .
    ```

2. Execute the following command to run the multi-container app,
    ```
    docker compose  -f my-stack.yaml up
    ```
3. To stop and delete all the containers created, execute the following command:
    ```
    docker compose  -f my-stack.yaml down
    ```
