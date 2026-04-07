# Uncertainty Engine SDK Template

Start using the SDK with an easy-to-use template and set-up guide. The template is accompanied by a detailed set of example workflows.

## Contents
- `template.ipynb` contains a simple template notebook to get up and running with the UE SDK
- `sdk_example` contains an SDK example, containing a number of commonly-used workflows

## Set-up

### 1. Clone Repository

Firstly, the contents of this repository should be cloned to your device.

- Select the green '<> Code' button
- If you have git installed on your device, clone the repository in your desired directory
- Otherwise, 'Download Zip' into the desired location

### 2. Configure Python Environment

The Uncertainty Engine SDK requires that you run Python version `>=3.10, <3.13`

Here is our guide to environment set-up iuf you are new to virtual environments:

Firstly, ensure that the approproate Python version is available on your device. Navigating to the sdk-example folder cloned in the previous step in your terminal, enter the follow into th create a virtual environment:

- For Mac/Linux:
    `python3.11 -m venv .venv`
- For Windows:
    `py -3.11 -m venv .venv`

This should create a folder in your version of the project called `.venv` with Python version 3.11 (or any other compatible version of your choosing) used as the interpretor. To activate this virtual environment, enter the following in your terminal:

- For Mac/Linux:
    `source .venv/bin/activate`
- For Windows:
    `.venv/Scripts/activate`

Once activated, each line in the terminal should now be preceeded by (.venv) on each subsequent line. If this does not change immediately, you may need to restart your terminal.

The benefit of using a virtual environment is that Python library inclusion and versioning can be contained to this project without affecting other projects on your device. 

Lastly, open the template.ipynb file in your cloned project and ensure that you can select `.venv` as a kernel

### 3. Install Dependencies 

In your terminal, with your virtual environment activated (each line should be preceeded by (.venv)), install the project dependencies using the following command:

`pip install -r requirments.txt`

### 4. Set UE Credentials

- Create a new file in the project directory called `.env'
- On separate lines set:
    - `UE_USERNAME=""`
    - `UE_PASSWORD=""`
- Save this file

NB: for those sharing notebooks via git, be sure to add a .gitignore to the project repo and to include .env. This will ensure that your credentials are not shared with other collaborators.

*You should now be sufficiently setup to run cells in the template and/or example notebooks available in this repository. Once you are familiar with the SDK interface, delete any unwanted notebooks (e.g., sdk_example.ipynb) and start building your own workflows*
