# Uncertainty Engine SDK Template

Start using the SDK quickly with this template repository, which is accompanied by a detailed set of exampkle workflows.

## Contents
- `template.ipynb` contains a simple template notebook to get up and running with the UE SDK.
- `sdk_example` contains an SDK example, containing a number of core workflows that can be facilitated by the UE

## Set-up

### Clone Repository

Firstly, the contents of this repository should be cloned locally.

If you have git installed on your device:
- Select the green '<> Code' button and clone this repository to your desired directory
    - `git clone ...` (HTTPS; SSH or CLI - depedning on your git set-up
 
If you don't:
- Simply 'Download Zip'

### Configure Python Environment

The Uncertainty Engine SDK requires that you run Python version `>=3.10, <3.13`

Here is our guide to environment set-up iuf you are new to virtual environments:

Firstly, ensure that the approproate Python version is available on your device (cd ...). Navigating to the sdk-example folder cloned in the previous step, enter the follow into the CMD line to create a virtual environment:

`python3.11 -m venv .venv`

This should create a folder in your verson of the project called `.venv`. To active this virtual environment, enter the following in your terminal:

`source .venv/bin/activate`

Your command line should now be preceeded by (.venv) on each subsequent line. If this does not change immediately, you may need to restart your terminal.

The benefit of using a virtual environment is that Python library inclusion and versioning can be contained to this project without affecting other projects on your device. 

Lastly, open the template.ipynb file in your cloned project and ensure that you can select `.venv` as a kernel

### Install Dependencies 

In your terminal, with your virtual environment activated (each line should be preceeded by (.venv)), install the project dependencies using the following command:

`pip install -r requirments.txt`

### Set UE Credentials

- Create a new file in the project directory called `.env'
- On separate lines set:
    `UE_USERNAME=""`
    `UE_PASSWORD=""`
- Save this file

Security Note: for those sharing notebooks via git, be sure to add a .gitignore to the project repo and to include .env. This should ensure your credentials are not shared directly with other collaborators
How to set up a venv
    How to make sure that we have the right version of Python.... (mac/windows/linux)

How to install all dependencies in requirements.txt
