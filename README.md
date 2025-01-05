# Spark with PySpark and JupyterLab

This guide provides a Docker Compose configuration for running PySpark alongside JupyterLab.

## Starting the Environment

To start the container, run:
```bash
docker compose up
```

The `notebooks` directory is mounted in the container, allowing you to access and save notebooks on your local machine.

The **JupyterLab** is available at [http://localhost:8888](http://localhost:8888).

The **Spark UI** is available at [http://localhost:4040](http://localhost:4040) after a Spark job is initiated.


The **JupyterLab token** is displayed in the logs of the JupyterLab container.

<div align="left">
<img src="https://github.com/user-attachments/assets/67023f79-ba2d-4686-8eec-16b70e797439" alt="Terminal Output" width="700">
</div>

## Using the Environment in VS Code

To integrate this setup with **Visual Studio Code**, follow these steps:

1. Open the root folder in VS Code and navigate to the `notebooks` directory.
2. Create a new Jupyter Notebook. In the top-right corner, use the **Select Kernel** option.
3. From the top menu, choose **Existing Jupyter Server…**
  <div align="left">
  <img src="https://github.com/user-attachments/assets/aa3e9c73-d84d-423c-b44b-d6d2bac9ac39" alt="Kernel Menu" width="500">
  </div>
  <br>

4. Select **Enter the URL of the running Jupyter Server…**
  <div align="left">
  <img src="https://github.com/user-attachments/assets/a030d780-a2e6-4f57-bd86-25d5067de062" alt="Server URL Option" width="500">
  </div>
  <br>

5. Input the server URL: [http://127.0.0.1:8888](http://127.0.0.1:8888), along with the token.
  <div align="left">
  <img src="https://github.com/user-attachments/assets/c683ea94-bdb8-4852-9d13-be786661cb4d" alt="URL Input" width="500">
  </div>
  <br>

6. Assign a custom display name for the server if desired.
  <div align="left">
  <img src="https://github.com/user-attachments/assets/6e6afa2b-bcd7-4662-b568-dc9c972d2162" alt="Display Name" width="500">
  </div>
  <br>

7. Choose **Python3 (ipykernel)** as the kernel.
  <div align="left">
  <img src="https://github.com/user-attachments/assets/6812ae03-bd7b-41e5-adcd-d04378a2d066" alt="Kernel Selection" width="500">
  </div>
  <br>

8. You can now run cells of your notebook and interact with the Jupyter server.
  <div align="left">
  <img src="https://github.com/user-attachments/assets/2823bd59-7145-4ed1-a8b5-a996e4768c8c" alt="VS Code Notebook" width="700">
  </div>
