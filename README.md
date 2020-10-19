# Interactive COVID-19 Data Visualizer
This notebook provides basic information about trends in COVID-19 hospitalizations and deaths in the US at the country, state and county levels. 

## Data Source
The data is provided by the New York Times, who gathers it based on reports from state and local health agencies. More information on the NYT dataset is available [here](https://github.com/nytimes/covid-19-data).

---
**NOTE**

Be sure to read the NYT's [explanation](https://github.com/nytimes/covid-19-data#geographic-exceptions) of some of the geographic exceptions in how they attribute data to certain cities and counties, especially if you are dealing with any of the following areas:

* New York City, NY
* Kansas City, MO
* Joplin, MO
* Alameda County, CA
* Douglas County, NE
* Chicago, IL
* Guam
* Puerto Rico
---

## Cloning the Repo
First, get a local copy of this repo:

> git clone https://github.com/DavidJBianco/covidtracker.git

This will create a new directory called _covidtracker_ under your current directory.  

The NYT COVID-19 data repository is included in this one as a Git submodule.  Before you can use it, though, you'll need to initialize the submodule. 

> cd covidtracker
> git submodule update --init

## Updating the Dataset
You'll want to re-download the newest copy of the NYT data every day.  To do this, you simply need to issue the following command from within the top-level directory:

> git pull --recurse --submodules

## Running the Notebook
Open the _covidtracker-use.ipynb_ file in Jupyter (either the Notebook or the Lab interface will work).  When you 'Run All Cells', the data will load and the initial visualizations will populate.  By default, it will generate cumulative and daily timelines for the US and for the state of Virginia.  Under the _Geographic Drill-Down_ section, you'll have the option to select a different state and, optionally, county for more detailed locality information.
