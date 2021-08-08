## _Dr. Sillystringz's Factory_

## _Description_

Dr. Sillystringz's Factory web application track machine repairs. This application
manages their engineers and the machine they are licensed to fix. The factory manager
is able to add a list of engineers when they are hired, a list of machines when they are bought and specify which engineers are licensed to repair a given machine(s) machine.

## _Technologies Used_

* C#
* ASP.NET Core MVC
* Entity Framework
* MySql Workbench
* HTTP RESTful Routing
* Git/GitHub

## _Setup Requirements_

* Browser
* Code Editor (preferrably vsCode)
* ASP.NET Core installed
* Terminal

## _Installation_

_Use the browser to navigate to GitHub page respository Click the Green Code button on the right and select Download Zip._

_Alternatively clone from Github via the terminal using ```git clone``` command In your terminal, navigate to the directory where you would like to clone the project to._

_Clone this repo to your chosen directory using this link ```https://github.com/godfreyowidi/dr.Sillystringzs_Factory``` in terminal._

* **Setting Up the Database**

_We use a tool called ```dotnet ef``` to create migrations and update database_

_Run ```$ dotnet tool install --global dotnet-ef --version 3.0.0``` globally in your terminal so that its available in all projects_

_Run the command ```dotnet build``` and all the necessary setup_

_We run the command ```$ dotnet ef migrations add Initial``` in the root directory of the project_

_Once we have verified that the migration, run the command ```$ dotnet ef database update``` to automatically update our database in MySQLWorkbench._

_Incase you made a mistake with the most the most recent migration and you haven't pushed the changes to Github. Run the command ```$ dotnet ef migrations remove``` to revert the migration._

* **.NET Environment Setup**

_After opening the project and before setting up the dependencies and tools for the project, add the file appsettings.json to the project root directory by running the command ```touch appsettings.json```. Click on the file and add the following:_
```
{
    "ConnectionStrings": {
        "DefaultConnection": "Server=localhost;Port=3306;database=[YOUR-USERNAME-HERE];uid=root;pwd=[YOUR-PASSWORD-HERE];"
    }
}
```
_This is a connection string and database will change based on which one we are connecting to. Replace [YOUR-USERNAME-HERE] and [YOUR-PASSWORD-HERE] with the name of your database schema and database login password_

_Because this file will contain sensitive information, it is imperative to add it to ```.gitignore`` file before making any commits_

* **If you chose to download via zip:**

_Unzip the downloaded repository into your working directory_

_Open the working directory into your code editor using the command ```code .```_

_Once you have the program open in your code editor, run ```dotnet restore``` inside the production directory to set up the dependencies and tools for the project._

_After the project is sucessfully set up, navigate to the directory in the terminal. Then execute the command ```dotnet run``` or ```dotnet watch run``` to start server_

* **If you cloned via Git:**

_Using the terminal, navigate to the directory the project is located using ```cd dr.Sillystringzs_Factory```_

_Open the working directory in your code editor using the ```code .``` command._

_From the terminal, ```run dotnet restore``` in the terminal to set up the dependencies and tools for the project._

_After the dependencies and tools for the project are sucessfully set up, navigate to the ```dr.Sillystringzs_Factory``` directory in the terminal._

_Execute the commmand ```dotnet run``` or ```dotnet watch run``` to start the server._

* **Using the application:**

_Server is started on either :-_

_http://localhost:5000_

_http://localhost:5001_

_Copy and paste either of the above in the browser to experience the splash page_

_You can follow along and add a machine and then assign an engineer to it._

_You can also search for specific machine and engineer using the unique ID_

_The application is also able to update and edit machines and engineers details as well as clear list of machines and engineers and also delete/destroy machines and engineers entries_

_Overally the application uses CRUD functionality as way to Create, Read, Update and Delete/Destroy information into persisent storage_


## _Known Bugs_
_no known bugs_

## _License_
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## _Contact_
[Email Contact](godfreyowiidi@gmail.com)