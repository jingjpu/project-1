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

---
## Contributors

```markdown

{
  "name": "Leigh Badua",
  "email": "leighbadua@gmail.com",
  "linkedin": "<>"
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