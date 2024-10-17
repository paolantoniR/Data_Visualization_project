# PROJECT FOLDER DESCRIPTION

The scripts in our project are enclosed into different repositories and numbered according to the order
they should be executed.
The following list will summarize the content of the project repository:

* **scraping** folder:
    * **webcrawlerrevised(1).py**: includes our web scraper (unfortunatelly not functional due to a restructuring of
      the crawled website) that collects the URLs of the csv datasets and saves them.
      into the *csvresources.txt* file
    * **datadownloading(2).py**: script that downloads the csv datasets thanks the URLs saved in
      the *csvresources.txt* file.
* **datasets_creation** folder:
    * **peopledataset(3).py**: script that creates a dataset in which each row represent a person/vehicle
      involved in an accident.
    * **accidentdataset(4).py**: script that creates a dataset in which each row represent an accident.
    * **DFCREATION(5).py**: script that creates the final datasets needed for the streamlit app.
    * **matchmunicipi(6).py**: script that matches each accident with a Rome suburb using latitude and longitude.
      (the geojson for the suburbs was taken from the [roma urbanistica](https://romaurbanistica.carto.com/tables/municipi/public)
      website)
* **loghi** folder: including all logos used in the website.
* **data** folder: including all the datasets used in the project.
* **Streamlitscripts** folder: The **MOST IMPORTANT** folder in the project, including
everything regarding our streamlit app, the format of this folder is standard for streamlit applications.
    * **pages** folder: includes the scripts for each page of the app.
    * **static** folder: including the backgrounds of the website.
    * **us** folder: including our pictures for the about us page.
    * **.streamlit** folder: including the configuration file for the streamlit app.
    * **Home.py**: the python script that needs to be ran to start the streamlit app.



# HOW TO RUN THE APP
Do the following steps:
1. Have a python environment that respects our **requirements.txt** file.
2. Open a terminal and navigate to the **Streamlitscripts** folder.
3. Run the following command: ``` streamlit run Home.py ```
4. The app will open in your default browser.
5. Enjoy the app!!!

Note: the scripts inside the **Streamlitscripts** folder cannot be executed with an interactive python 
console due to the way in which relative paths are handled by streamlit. 

# CONTRIBUTORS

* Luigi Colonna

* Mattia Cervellini

* Emanuele Rosati

* Riccardo Paolantoni
