# CIT Console Template
An opinionated F# Console application template.

## Features
* `global.json` pinned to .NET 8
* VS Code settings to hide inlay hints by default
* `.gitignore` with common F# settings
* Standard `src/<app>` folder structure
* **Fantomas v6** pre-configured with `.editorconfig`
* **Paket v8** with the following dependencies:
    * FSharp.Core
    * FSToolkit.ErrorHandling

## To install locally
```bash
dotnet new install .\
```

## To run
```bash
dotnet new cit-console
```