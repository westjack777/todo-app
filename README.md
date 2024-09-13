# ToDo App
A simple ToDo App using React, .NET Core and SQL Server.  
Using this app, you can add and remove notes.


## I. Pre-requirement
### 1. Node JS
Get **Node JS** from [here](https://nodejs.org/en/download).  
**Note**: Don't forget to add Node JS to your environment variable's `PATH` 

### 2. Install SQL Express
Get **SQL Express** from [here](https://www.microsoft.com/en-us/sql-server/sql-server-downloads).  
**Note**: Additionally you can select to install the SSMS to manage your SQL Database. Use the script below to create the database.  
  
**Note 2**: Remember to set the DefaultConnection on the `api\ToDoApp\ToDoApp\appsettings.json` file!
```
CREATE DATABASE ToDoApp;

USE ToDoApp;

CREATE TABLE dbo.Notes (
    id BIGINT IDENTITY(1,1) PRIMARY KEY,
    [description] NVARCHAR(MAX)
);
```

### 3. Install .NET SDK
Get **.NET SDK** from [here](https://dotnet.microsoft.com/download).  
**Note**: Don't forget to add .NET SDK to your environment variable's `PATH` 


## II. Run the project
From a command prompt window:
- Clone the project `git clone https://github.com/westjack777/todoapp.git`
- Navigate to `todoapp\api\ToDoApp\ToDoApp` and run `dotnet run`.
- Navigate to `todoapp\ui` and run:  
```
  npm install
  npm start
```

