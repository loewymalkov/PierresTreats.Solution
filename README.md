# PIERRESTREATS

Web page to add treats and flavors to a database. 

## USE

A web page that allows a user to create an account and add/store treats and flavors. App can keep track of multiple treats, multiple flavors and multiple associations between them, i.e. a 'caramel' treat can have the flavors 'sweet' and 'salty'. Built for Epicodus C# track, project built to learn user authentication and authorization with a web application. 

## SET-UP

- from terminal, run 'git clone https://github.com/loewymalkov/PierresTreats.Solution'
- navigate to project directory 'PierresTreats' and enter 'dotnet restore', 'dotnet ef database update'
- to use the web app, enter 'dotnet watch run' or 'dotnet run' to launch server, make sure you have follow instructions to set up database


## SPECS

The application should have user authentication. A user should be able to log in and log out. Only logged in users should have create, update and delete functionality. All users should be able to have read functionality.
There should be a many-to-many relationship between Treats and Flavors. A treat can have many flavors (such as sweet, savory, spicy, or creamy) and a flavor can have many treats. For instance, the "sweet" flavor could include chocolate croissants, cheesecake, and so on.
A user should be able to navigate to a splash page that lists all treats and flavors. Users should be able to click on an individual treat or flavor to see all the treats/flavors that belong to it.

| Behavior | Input | Output |
|-|-|-|
| user should be able to create an account | 'create account' | _navigates to register page_ |
| user should be able to register| 'username: xxxxx@xxxx.com password:xxxxx' | _creates username with password and stores in database_ |
| user should be able to log in | 'username: xxxxx@xxxx.com, password:xxxxx' | _authenticates user, redirects to account index_ |
| user should be able to log out | 'log out' | _logs user out, redirect to account index_ |
| user needs account to be authorized to create, update and delete | 'create new treat' | _checks user authorization to create a new treat_ |
| user should be able to add treats | 'Caramel' | _adds 'Caramel' to treats table_ |
| user should be able to add flavors | 'Sweet' | _adds 'Caramel' to flavors table_|
| user should be able to add a flavor to a treat | 'Add Sweet to Caramel' | _updates relationship between treat and flavor for those items_ |
| user should be able to add many flavors to a treat | 'Add Salty to Caramel' | _updates relationship between treat and flavor for those items_ | 

## TECHNOLOGIES

C#, cshtml, MySQL, EntityFramework, VS Code;

## AUTHOR

Loewy Malkovich, loewymalkov@gmail.com
Oct. 2019

## LICENSE

Open source (2019)