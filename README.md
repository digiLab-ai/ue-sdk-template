# Uncertainty Engine SDK Template

This guide will help you get started with the Uncertainty Engine (UE) SDK using a simple template and step-by-step setup instructions. The template is accompanied by a detailed example that utlises some commonly used workflows.

## Contents
- `template.ipynb` – A simple notebook template to get up and running with the UE SDK  
- `sdk_example` – Example workflows demonstrating commonly used SDK functionality  

---

## Set-up Guide

### 1. Clone the Repository

First, clone this repository to your local machine:

- Click the green **“<> Code”** button on the repository page  
- If you have Git installed, clone the repository into your desired directory  
- Otherwise, select **“Download ZIP”** and extract it to your chosen location  

---

### 2. Configure Your Python Environment

The Uncertainty Engine SDK requires **Python version `>=3.10, <3.13`**.

If you're new to virtual environments, follow these steps:

1. Ensure a compatible Python version (e.g. 3.11) is installed on your system  
2. Open a terminal and navigate to the `sdk_example` folder from the cloned repository  
3. Create a virtual environment:

#### Mac/Linux
```bash
python3.11 -m venv .venv
```

#### Windows
```bash
py -3.11 -m venv .venv
```

This will create a `.venv` folder using Python 3.11 (or another compatible version of your choice).

#### Activate the Virtual Environment
#### Mac/Linux
```bash
source .venv/bin/activate
```

#### Windows
```bash
.venv/Scripts/activate
```

Once activated, your terminal prompt should be prefixed with (.venv). If not, try restarting your terminal.

*Why use a virtual environment?*
It isolates project dependencies, preventing conflicts with other Python projects on your system.
Finally, open template.ipynb and ensure that .venv is selectable as the notebook kernel.

--- 

### 3. Install Dependencies 

Withe the virtual environment activated, install the required dependencies:

```bash
pip install -r requirments.txt
```

---

### 4. Set UE Credentials

1. Create a new file in the project directory called `.env'
2. Add the following, along with your UE credentials:
```bash

UE_USERNAME=""
UE_PASSWORD=""

```
3. Save this file

> #### Important
> If you are sharing this repository (e.g. via Git), ensure that .env is included in your .gitignore file to prevent exposing credentials.

---

### Next Steps
You are now ready to run the notebooks in this repository.
- Start with template.ipynb for a basic workflow
- Explore sdk_example for more advanced usage patterns
Once you're comfortable with the SDK, you can remove example notebooks and begin building your own workflows.
