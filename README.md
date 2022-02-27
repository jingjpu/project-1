# crypto_realestate_v2
A first step towards Crypto enabled Settlements

## Executive Summary

An Early Stage Online Marketplace for New Homes* has buyers who wish to transact in crypto and sellers who wish to settle in USD
New Homes are distinct use case because there is presently no efficient way to hedge (insure) crypto denominated contracts 10-18 months.
Company is current leader in new home Marketplace and would to maintain edge for home purchases using Crypto.

First step and project goal is to convert all homes prices from USD to BTC/ETC and explore what it might cost to transact using Crypto.

### Data Collection and Cleanup

House Price obtained from company API and currency info from FTX.  (FTX is industry leader in crypto derivatives.)
Home Price Data Obtained from company mySQL dump - cleanup process included removing data privacy concerns, locating relevant tables, and requesting additional information from company on the data schema and relationships.


## Technologies

This crypto realester tool is a Jupyter notebook built with the following technologies:

### Language

| Language | Version |
|----------|---------|
| Python   | 3.7.11  |

### Libraries and Frameworks

| Component | Version |
|-----------|---------|
| Anaconda  | 1.9.0   |
| Conda     | 4.11.0  |
| Jupyter   | 3.2.1   |

### Operating System

This version of the software is operating system agnostic.

---
## Installation Guide

### Pre-requisites

- Python 3.7
- Anaconda 1.9.0
- Conda 4.11.0
- Jupyter 3.2.1
- A conda environment created specially for this project.


### Required Python Packages

| Package    | Purpose                                                                                                                                                        |
|------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| datetime   | Basic date and time types                                                                                                                                      |
| dotenv     | Reads key-value pairs from a .env file and can set them as environment variables                                                                               |
| hmac       | Provides secure hash functions                                                                                                                                 |
| holoview   | make data analysis and visualization seamless and simple                                                                                                       |
| hvplot     | A high-level plotting API for the PyData ecosystem built on HoloViews                                                                                          |
| ipykernel  | Python execution backend for Jupyter                                                                                                                           |
| ipywidgets | Also known as jupyter-widgets/widgets, are interactive HTML widgets for Jupyter notebooks and the IPython kernel                                               |
| json       | Simple JSON decoder.                                                                                                                                           |
| matplotlib | comprehensive library for creating static, animated, and interactive visualizations                                                                            |
| numpy      | adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions to operate on these arrays |
| os         | Miscellaneous operating system interfaces                                                                                                                      |
| pyviz      | an open platform for helping users decide on the best open-source (OSS) Python data visualization tools                                                        |
| requests   | simple HTTP library for Python                                                                                                                                 |
| streamz    | Streamz helps you build pipelines to manage continuous streams of data                                                                                         |
| time       | Time access and conversions                                                                                                                                    |


### Running the Analyzer

Install a new conda environment for this project. We will be using `python 3.7.11` for this repository.

```bash
conda create -n dev_crypto_realestate python=3.7.11 anaconda
```

Activate the newly created environment and verify the python version.

```bash
conda activate dev_crypto_realestate
python --version
```

Install and add the ipykernel environment to your jupyter notebook.

```bash
conda install -c anaconda ipykernel
python -m ipykernel install --user --name=dev_etf

```

Install the required python packages.

```bash
conda install hvplot, streamz, holoviews
conda install -c conda-forge streamz
conda install -c conda-forge holoviews
conda install hvplot
conda install -c conda-forge pyviz
conda install -c conda-forge python-dotenv
conda install -c pyviz panel
conda install -c pyviz geoviews
```

Clone the remote repository to your local developer environment and `cd` into the folder.
```bash
git clone git@github.com:msashokkumar/crypto_realestate_v2.git
cd crypto_realestate_v2
```

Start the jupyter lab server from the terminal as follows:

```bash
jupyter lab
```

Open and execute the file `crypto_realestate_v2.ipynb`


This crypto realester tool uses an `.env` file to store FTX API key and secret keys. To use this tool, create and login to [FTX US exchange](https://ftx.us/profile) to access your trading API keys. Then create an `.env` file to your remote repository on your local environment with the following syntex below:
```
ftx_api_key=<your_api_key>
ftx_secret_key=<your_secret_key>
```

---
## Usage

Project library imports:
<img width="1107" alt="01_project_library_imports" src="https://user-images.githubusercontent.com/96001018/155888148-ddafbe00-cde9-424a-9c4e-1210ac42874f.png">


Home Price Data obtained from company mySQLdump. Collection process included data privacy concerns, locating relevant tables, and requesting additional information from company. DataFrame Preparation (column selection, drop, and merge DataFrames).
<img width="899" alt="02_units_df" src="https://user-images.githubusercontent.com/96001018/155888149-07f048c1-e02a-4ccf-9a05-c85a387557cb.png">


Using hvplot to visualize real estate property listing across the United States. User can use interactive widgets to pan, zoom, and hover over marked points for more property information:<n>

<img width="562" alt="03_all_units_geo_view" src="https://user-images.githubusercontent.com/96001018/155888154-7e344d5f-45ae-4a68-89e4-1dd12aae9691.png">


Interactive display that allows for the User to filter through property status (available, reserved, sold, & unreleased) and location by city. Results of the search will populate property ID and price (on left) and a corresponding geoview map (on right).

<img width="1118" alt="04_available_units_in_locality" src="https://user-images.githubusercontent.com/96001018/155888155-650fe329-77ac-4e2a-8aa1-4d17fd65800c.png">

 
  
Live requests are made to the FTX Exchange for BTC's most current value. 

<img width="1253" alt="05_live_btc_value_for_all_units" src="https://user-images.githubusercontent.com/96001018/155888157-3637ac56-0021-4ccd-9574-5ff89226c508.png">

  
Lastly, the User is able to select the a property by ID. Prices for cryptocurrency (BTC) is fetched and updated every 15 seconds. 
<img width="1208" alt="06_live_btc_value_chart_for_selected_unit" src="https://user-images.githubusercontent.com/96001018/155888159-750ca69a-15d3-4e7b-924a-cb11d3e18cb3.png">

---
## Contributors

```markdown

{
  "name": "Leigh Badua",
  "email": "leighbadua@gmail.com",
  "linkedin": "<www.linkedin.com/in/leighbadua>"
},
{
  "name": "Rebecca Brown",
  "email": "beccabeastly@gmail.com",
  "linkedin": "<>"
},
{
  "name": "Jing J Pu",
  "email": "jingjpu@gmail.com",
  "linkedin": "<>"
},
{
  "name": "Ashok Kumar Madhavi Selvaraj",
  "email": "ashok.ms.kumar@gmail.com",
  "linkedin": "https://www.linkedin.com/in/msashokkumar"
}
```
---

## License

Please refer to LICENSE.
