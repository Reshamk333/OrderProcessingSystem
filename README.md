The Order Processing System is a .NET Core application designed to handle order processing workflows. 

1. Project Setup Instructions
Prerequisites
Operating System: Windows 10 (Version 22H2 or later) 
Tools Required:
Visual Studio 2022
.NET SDK 7.0+
SQL Server (local instance).

2. Setup Steps
Clone the Repository
git clone https://github.com/Reshamk333/order-processing-system.git


3. Update database connection - DefaultConnection in appsettings.json
4. Apply Migrations Run the following commands to set up the database:
  a. Add-Migration InitialCreate
  b. Update-Database
  c.dotnet ef database update

5. Api end poins
  a. api/Customers - to get all customers details - http://localhost:5242/api/Customers/1
  b. api/Customers/{id} - to get a customer detail base on id - http://localhost:5242/api/Customers
  c. api/Orders/{customerId} body{productIds} - to save order details for customer id - http://localhost:5242/api/Orders?customerId=3 {body} [1, 2, 3]
  d. api/Orders/{orderid} - to get order details base on id - http://localhost:5242/api/Orders/1
