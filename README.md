## Superset Cloning Tool

## Partner Intro:
Our primary point of contact for this project is Evan Wheeler (ewheeler@unicef.org). 

UNICEF is a multinational organization dedicated to protecting, assisting, and creating environments for children to grow up with the resources they need. They make data-driven decisions and support humanitarian efforts worldwide. 

## Project Description
We will be building a web interface for the existing command line proof of concept that clones Apache Superset dashboards. Users will have the ability to modify and clone existing dashboards. Additionally, new features, such as a version control that would allow for the propagation of changes from the configuration to the parent dashboard to the cloned children. The current problem is difficulty surrounding the use of the cloning tool and redundant testing for staging and production environments, and so with these additions, UNICEF employees, and other Superset users, will have the tools to quickly and easily visualize whatever data they want. This application will unlock the opportunity for larger teams to work together on dashboards across the globe, rather than individual users having their own instances on their accounts.
   
## Key Features
Our primary feature is a web interface that would allow users to clone a dashboard template and populate it with any compatible datasource. Additional features include a version control system that would allow a user to make changes to a dashboard's configuration and update the cloned dashboards. In addition to being able to clone dashboards within the same instance we plan to implement cloning across superset instances.

Feature Breakdown
* Login Interface and Authentication

The user will be required to specify a URL to their instance of superset, as well as their username and password for authentication.

* View all existing dashboards, charts, and datasets in their instance of Superset

The user will be able to view all the dashboards they have available to clone from in their instance of superset. Upon selecting a dashboard, the user will be able to view all charts and datasets they have available to populate.

* Cloning a Dashboard

The user will be able to choose an existing dashboard as the starting template. Once this dashboard is chosen, the user will be required to select a dataset for each of the existing charts that are part of the template dashboard. The user will be given the option to rename the cloned dashboard and any of the available charts.

* Version control to update all cloned dashboards when prompted to the original dashboard

Upon cloning a dashboard, all changes will be tracked in the database. This will allow users to push those changes onto dashboards that were previously cloned from the original modified dashboard.

## Instructions
### Instructions To Run the App

Follow the link provided below:

https://project12-csc301.onrender.com/

Login to the program using the following credentials:

Dashboard Name: User

Superset Username: testuser

Superset Password: testpass

On the main screen, the user will be able to select any dashboard to clone. Clicking on one of these dashboards, will take the user to the cloning page.

Here they will have the option to rename their dashboard, view the names of all charts, and select the dataset for each of the charts. Then the user will click on the clone button. 
For the current version of the program select only the dataset that corresponds to the selected dashboard for all charts.

Ex. If the dashboard (Covid Vaccines) was selected, select the dataset (covid vacinnes) for all chart instances.

The cloned dashboard will be ready and viewable on superset. The user will then be sent back to the main screen.

To go on Superset:

Link: https://superset-dev.unicef.io/

Username: admin

Password: UNICEFToronto2023##

### Instructions to Work on the Project

For more detailed instructions view README-dev.md

Prior to working on the backend, make sure that you create a virtual environment in the backend folder. To do so, first navigate to the backend directory, and then type the following command:
```
python -m venv venv
(If this does not work try: py -m venv venv)
```
Once the venv folder has been created, activate the environment:
```
(MacOS) source venv/bin/activate
(Windows) .\venv\Scripts\activate
(if errors occur try switching from \ to / and vice-versa)
```
If the folder contains a requirements.txt, install all required (Python) libraries using the requirements.txt after you've created the venv. 
```
pip install -r requirements.txt
```
Before pushing, ensure that if you've downloaded new libraries, you create a new requirements.txt by running the command:
```
pip freeze > requirements.txt
```
The instructions above are for MacOS/Linux; for Windows, read this article on how to do this: [Python Virtual Environments: A Primer – Real Python](https://realpython.com/python-virtual-environments-a-primer/)

## Licences 
We will be using an MIT licence. UNICEF values contributing to the open source community. Our partner believes that this project will not only be useful for UNICEF, but will also be desired by other companies. Therefore, we have received permission to upload the code on GitHub and share it freely.

### Contributors
Special thanks to:
- Nicholas Macasaet
- Rohan Mistry
- Manya Mittal
- Rudraksh Monga
- Andrew Nguyen
- Jessica Zhang
