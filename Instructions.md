# Instructions

## Contents
In addition to the files included in the original test, you will find the following files in my GitHub repository.

 - Instructions.md. It is this document. It details the material and the steps to be followed to reproduce the solution.
 - [requirements.txt.](https://github.com/merce78/data-science-test-solution/blob/main/requirements.txt) This file includes the lists of python packages required to run the code proposed. It's used only to setup the environment.
 - [data_simulation.ipynb](https://github.com/merce78/data-science-test-solution/blob/main/data_simulation.ipynb). Notebook used to generate the simulated data. This notebook is self-explanatory.
 - [data/rpc_rents.csv.](https://github.com/merce78/data-science-test-solution/blob/main/data/rpc_rents.csv) CSV containing the simulated data generated in the previous code..
 - [solution_dev.ipynb](https://github.com/merce78/data-science-test-solution/blob/main/solution_dev.ipynb). Notebook used to solve the test using the simulated data. 
 - [IFCO Findings.pdf.](https://github.com/merce78/data-science-test-solution/blob/main/IFCO%20Findings.pdf) Basic presentation to report our findings to the stakeholders.

 

## Setup environment

I used VSCode  and python 3.12 to generate the code and materials. 
Code is in Jupiter notebook for clarity as notebooks allow to add markdown texts.
I assume git, python and VSCode (or equivalent) with Jupiter Notebook plugins  are already installed.
These are the steps to follow in order to reproduce the steps and use the materials. 

 

 1. Open a terminal and clone the github repository: [https://github.com/merce78/data-science-test-solution.git](https://github.com/merce78/data-science-test-solution.git) and access to it.

    git clone  https://github.com/merce78/data-science-test-solution.git
    cd data-science-test-solution

 2. Create a virtual python environment to work with and activate it. (linux command)

    python3 -m venv env
    
    source env/bin/activate

 4. Install python packages 

    pip install -r requirements.txt

 5. Open the folder in VSCode or equivalent and ensure the python kernel you're using is the one that  you just created. (env)


## First step:  Generate simulated data

By simulating some data we can better understand the problem and it will help us to explain and validate the solution.

For this step you can use data_simulation.ipynb which is a self-explanatory notebook. The output will be a CSV file with 4 fields that will be stored in the data directory.

Please note that if you run the code without modifying the output CSV name, you will overwrite the generated data which may cause the conclusions to change slightly in the next step.

## Second step: Solve scenario 1 questions.

The input for this step will be the CSV with simulated data generated earlier. 
The code to follow the solution is in solution_dev.ipynb notebook which is also self-explanatory. 
At the end of this notebook you can also find some charts and calculations used later in the presentation to stakeholders.

## Third step: Present findings to non-technical stakeholders.
In IFCO_Findings.pdf  there is a basic presentation as support to explain our conclusions to the stakeholders.
