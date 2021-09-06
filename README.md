# Blog with ASP.NET Core and React/Redux

# Blog Api

## Requirements:
 - .NET Core 2+
 - PostgreSQL(connection string specified in Blog.API/appsettings.json)

## Example of how to create a database user
```bash
sudo -i -u postgres
psql
create user blogadmin;
alter user blogadmin with password 'blogadmin';
alter user blogadmin createdb;
```

## Run locally
```bash
git clone
cd backend
cd Blog.API
dotnet ef database update
# if you want to populate the database with mock data
# start
cd ..
cd Blog.Mocker
dotnet run
cd ..
cd Blog.API
# end
dotnet run 
```