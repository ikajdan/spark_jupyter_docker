# Spark with PySpark and JupyterLab

This guide provides a Docker Compose configuration for running PySpark alongside JupyterLab.

## Starting the Environment

To start the container, run: `docker compose up`. The `notebooks` directory is mounted in the container, allowing you to access and save notebooks on your local machine.

The **JupyterLab** is available at [http://localhost:8888](http://localhost:8888).

The **Spark UI** is available at [http://localhost:4040](http://localhost:4040) after a Spark job is initiated.


The **JupyterLab token** is displayed in the logs of the JupyterLab container.

<div align="left">
<img src=".figures/terminal.png" alt="Terminal Output" width="700">
</div>

## Using the Environment in VS Code

To integrate this setup with **Visual Studio Code**, follow these steps:

1. Open the root folder in VS Code and navigate to the `notebooks` directory.
2. Create a new Jupyter Notebook. In the top-right corner, use the **Select Kernel** option.
3. From the top menu, choose **Existing Jupyter Server…**

<div align="left">
<img src=".figures/menu1.png" alt="Kernel Menu" width="500">
</div>
<br>

4. Select **Enter the URL of the running Jupyter Server…**

<div align="left">
<img src=".figures/menu2.png" alt="Server URL Option" width="500">
</div>
<br>

5. Input the server URL: [http://127.0.0.1:8888](http://127.0.0.1:8888), along with the token.

<div align="left">
<img src=".figures/menu3.png" alt="URL Input" width="500">
</div>
<br>

6. Assign a custom display name for the server if desired.

<div align="left">
<img src=".figures/menu4.png" alt="Display Name" width="500">
</div>
<br>

7. Choose **Python3 (ipykernel)** as the kernel.

<div align="left">
<img src=".figures/menu5.png" alt="Kernel Selection" width="500">
</div>
<br>

8. You can now run cells of your notebook and interact with the Jupyter server.

<div align="left">
<img src=".figures/vscode.png" alt="VS Code Notebook" width="700">
</div>
