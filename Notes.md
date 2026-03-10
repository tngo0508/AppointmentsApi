
```shell
dotnet add package Microsoft.EntityFrameworkCore
dotnet add package Microsoft.EntityFrameworkCore.Sqlite
dotnet add package Microsoft.EntityFrameworkCore.Tools

dotnet tool install --global dotnet-ef
dotnet ef migrations add InitialCreate
dotnet ef database update

dotnet tool install --global dotnet-aspnet-codegenerator
dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design
dotnet aspnet-codegenerator controller -name AppointmentsController -async -api -m Appointment -dc AppointmentContext -outDir Controllers -dbProvider sqlite
```

