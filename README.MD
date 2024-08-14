# Getting started

Run the init-script.sh to get the dependencies and test the build

```
dotnet add package log4net
dotnet add package Microsoft.Extensions.Logging.Log4Net.AspNetCore
```

Add the log4net provider in the app build - See Program.cs

```
// Add services to the container.
builder.Logging.ClearProviders();
builder.Logging.AddLog4Net("log4net.config");
```

Log some stuff in controller - See WeatherForecastController.cs

```
_logger.LogInformation("WeatherForecast endpoint was called");
```

Hit the Pink Palace with a fist full of pineapples...
