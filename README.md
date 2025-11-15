# B1SAAPI
B1SA Technical Assessment


The NumberWord API is an ASP.NET Core 9 Web API that analyzes English number words in a string (e.g., "onetwoten") and returns structured results.  
It also includes a random number-word generator endpoint (generates valid word number string) used for testing and demo purposes.
This document describes how to set up, run, and test the project.

##  Requirements
Before running the project, ensure you have:
- NET 9 SDK
- Visual Studio 2022 (or newer) 
- Serilog NuGet packages installed:
  - Serilog
  - Serilog.Sinks.File
- Windows, Linux, or MacOS supported
- ABP Framework already integrated in the project (no extra steps needed)

##  Project Setup

1. Clone the repository
Restore all NuGet packages

Commands
1.	dotnet restore
2.	dotnet build
Ensure the required Serilog packages exist
If missing, install manually:
1.	dotnet add package Serilog
2.	dotnet add package Serilog.Sinks.File



Run Application

Swagger will show:
1.	/api/numberword/analyze
2.	/api/numberword/generate-random

ABP built-in endpoints:

1.	/api/abp/api-definition
2.	/api/abp/application-localization
3.	/api/abp/application-configuration

 Running Tests
The solution includes xUnit tests.
Run all tests from command line:
1.	dotnet test



