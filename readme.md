# CIT F# Application Template
An opinionated F# application template.

## Features

### Configuration
* `global.json` pinned to .NET 8
* **VS Code** settings to hide inlay hints by default
* `.gitignore` with common F# settings
* Standard `src/<app>` folder structure

### Pre-installed dotnet tools
* **Fantomas v6** pre-configured with `.editorconfig`
* **Paket v8** with the following dependencies:
    * FSharp.Core
    * FSToolkit.ErrorHandling

### Console App
* Comes with a single standard console application

## To install locally
```bash
dotnet new install .\
```

## To run
```bash
dotnet new cit-console
```
