1. Update database connection - DefaultConnection in appsettings.json
2. Data migration 
  a. Add-Migration InitialCreate
  b. Update-Database
3. Api end poins
  a. api/Customers - to get all customers details
  b. api/Customers/{id} - to get a customer detail base on id
  c. api/Orders/{customerId} body{productIds} - to save order details for customer id
  d. api/Orders/{orderid} - to get order details base on id
