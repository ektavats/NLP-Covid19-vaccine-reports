# Exploring Covid-19 and non-Covid vaccine reports using NLP
This work explores Covid-19 and non-Covid vaccine reports from VAERS2020 database using NLP

## Dataset: <br>
Reports from VAERS, 2020. Download link: https://vaers.hhs.gov/data/datasets.html.

### Dataset description:

Type of file: CSV

2020VAERSData.csv : contains information about vaccine data including symptom narratives (column SYMPTOM_TEXT). There exist other free-text fields on the reports. It has 35 columns and 5352 rows

2020VAERSVAX.csv : contains vaccine information. It has 8 columns and 5472 rows. Column VAX_NAME contains the vaccine name for the report and one can identify the COVID19 reports using this column.

Both files contain a unique ID VAERS_ID for linking the tables.

The data is from the US in 2020, and includes reports for Covid-19 vaccines and other vaccines.

## Set up:<br>

Create a new virtual environment and install all the necessary Python packages: 

conda create --name env_name python=3.8 pip numpy pandas matplotlib seaborn altair jupyterlab 
conda activate env_name 
pip install wordcloud

For ScispaCy (Mac): 
CFLAGS="-mavx -DWARN(a)=(a)" pip install nmslib  pip install scispacy

For ScispaCy (Windows):  pip install scispacy

## Contact: <br>

Ekta Vats <br>
Centre for Digital Humanities, Department of ALM, Uppsala University <br>
ektavats@gmail.com <br>
