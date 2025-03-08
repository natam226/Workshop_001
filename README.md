
# Workshop 001

In this workshop we use a dataset of randomly generated data, that contains information about candidates who participated in selection processes. The dataset contains 50.000 rows and 10 columns, that are going to be used to analyze specific metrics through charts. 

The technologies used are:
- *Python*
- *Jupyter Notebook*
- *PostgreSQL*
- *PowerBI Desktop*

The libraries used are:
- *Pandas*
- *SQLAlchemy*
- *Matplotlib*
- *Numpy*
- *Seaborn*

## Columns information
This dataset contains 10 columns with the following information:
- First Name
- Last Name
- Email
- Country
- Application Date
- Yoe (years of experience)
- Seniority
- Technology
- Code Challenge Score
- Technical Interview Score

### Clone the repository
Execute the following command to clone the repository

```bash 
git clone https://github.com/natam226/Workshop_001.git

```

> From this point on all processes are done in Visual Studio Code

### Create Virtual Environment
To create a virtual environment you should use the following command
```bash
python -m venv venv
```
To activate the virtual environment you should move to the `venv/Scripts` folder an run the following command to activate the virtual environment
```bash
activate
```

### Credentials
To make a connection to the database you must have the database credentials in a JSON file called credentials. So this file must be created in the project folder, with the following syntax:

```bash
{
    "db_host": "DB_HOST",
    "db_name": "DB_NAME",
    "db_user": "DB_USER",
    "db_password": "DB_PASSWORD",
    "db_port": "DB_PORT"    
}

```
### Installing the dependencies
The necessary dependencies are stored in a file named requirements.txt. To install the dependencies you can use the command
```bash
pip install requirements.txt
```
### Run the notebooks
You execute the three notebooks by the following order:

1. 001_raw_data_load.ipynb
2. 002_EDA.ipynb
3. 003_clean_data_load.ipynb

The correct python kernel must be chosen to run correctly

### Connecting the database with PowerBI

1. Open PowerBI desktop and create a new file. Select *Get data* and choose the way you want to import the data. In this case is going to be *PostgreSQL Database*.

2. Insert the PostgreSQL server and database name, and press *Accept*.

3. Fill in the fields with the credentials, and press *Accept*.

4. When you're connected to the database you will be able to select the table with the clean data to start creating the dashboard. 