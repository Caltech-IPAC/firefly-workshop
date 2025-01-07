# Firefly Workshop
Tutorial notebooks on using the Firefly Python client (and Jupyter Lab extension)
to visualize astronomical data as images, tables, charts, and more!

## Setup Workshop Environment

### Prerequisites
If you don't have the following installed already,
- **miniconda**: Install by following the steps at https://docs.anaconda.com/miniconda/install/#quick-command-line-install
- **git**: Install from https://git-scm.com/downloads

> Note: If you're using Windows, it is *highly recommended* to use [Windows 
Subsystem for Linux (WSL)](https://learn.microsoft.com/en-us/windows/wsl/install)
for fewer installation headaches. 

### Setup instructions
1. Clone this repository on your machine:
    ```sh
    git clone https://github.com/Caltech-IPAC/firefly-workshop
    cd firefly-workshop
    ```

2. Create Python environment with all the necessary dependencies including Firefly Python client and Jupyter Lab extension:
    ```sh
    conda env create --file environment.yml
    conda activate firefly-py-env
    ```
    The name of the new conda environment created above should be displayed next to the terminal prompt:
    ```
    (firefly-py-env)
    ```

3. Set the environment variable for Firefly server to let the Firefly Jupyter Lab extension know which server to talk to from the Python client. We use a public Firefly server - IRSA Viewer:
    ```sh
    export FIREFLY_URL=https://irsa.ipac.caltech.edu/irsaviewer
    ```

4. Open the exercise notebooks in Jupyter Lab:
    ```sh
    cd exercises
    jupyter lab
    ```


## Exercises

We have 3 notebooks demonstrating how to visualize astronomical data from Python
using Firefly in [exercises](exercises/) directory:
- [Using Firefly to Explore OpenUniverse2024 Data Preview Simulated Roman and Rubin Images](exercises/OpenUniverse2024Preview_Firefly.ipynb)
- [Using Firefly visualization tools in Python to vet SEDs](exercises/SEDs_in_Firefly.ipynb)
- [Using Firefly visualization tools to understand the light curves of Solar System objects](exercises/NEOWISE_light_curve_demo.ipynb)


## Solutions

The solutions of the above exercise notebooks are present at [Firefly section in
IRSA Tutorials](https://caltech-ipac.github.io/irsa-tutorials/#interactive-visualization-in-python-with-firefly) website.


## Reference/Cheatsheet

Once you have completed the setup instructions above, you are ready to visualise
your data files from python in Firefly using the Firefly Python client.
To learn how to use Firefly Python client (`firefly_client` package), you can
explore its [documentation website](https://caltech-ipac.github.io/firefly_client/index.html).


The following is a condensed list of all those pages that are most relevant for 
this workshop:
- [FireflyClient API reference](https://caltech-ipac.github.io/firefly_client/api/firefly_client.FireflyClient.html):
You can use "Methods Summary" table to navigate to learn about the function
you are interested in and its parameters.
- [Displaying Images using Firefly client](https://caltech-ipac.github.io/firefly_client/usage/displaying-images.html)
- [Visualizing Tables and Catalogs using Firefly client](https://caltech-ipac.github.io/firefly_client/usage/viewing-tables.html)
- [Visualizing ds9-style Regions using Firefly client](https://caltech-ipac.github.io/firefly_client/usage/overlaying-regions.html)
- [Making Plots using Firefly client](https://caltech-ipac.github.io/firefly_client/usage/charting.html)

