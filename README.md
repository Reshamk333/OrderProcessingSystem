1. Update database connection - DefaultConnection in appsettings.json
2. Data migration -
  1. Add-Migration InitialCreate
  2. Update-Database
3. Api end poins
  1. api/Customers - to get all customers details
  2. api/Customers/{id} - to get a customer detail base on id
  3. api/Orders/{customerId} body{productIds} - to save order details for customer id
  4. api/Orders/{orderid} - to get order details base on id
