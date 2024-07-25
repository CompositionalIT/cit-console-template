# CIT F# Application Template
An opinionated F# application template.

## Features

### Configuration
* **global.json** pinned to .NET 8
* **VS Code** settings to hide inlay hints by default
* **.gitignore** with common F# settings
* **src/app** folder structure
* **Directory.Build.props** file to enforce treating warnings as errors

### Pre-installed dotnet tools
* **Fantomas v6** pre-configured with `.editorconfig`
* **Paket v8** with the following dependencies:
    * FSharp.Core
    * FSToolkit.ErrorHandling

### Console App
* Comes with a single standard console application
* Comes with a solution file (seems to help Ionide finding the project for highlighting).

## To install locally
```bash
dotnet new install ./
```

## To execute the template
```bash
dotnet new cit-app -o MyApp
```

will give you a folder structure as follows:

```
.config
    dotnet-tools.json
.paket
    Paket.Restore.targets
.vscode
    settings.json
src
    MyApp
        MyApp.fsproj
        paket.references
        Program.fs
MyApp.sln
.editorconfig
.gitignore
Directory.Build.props
global.json
paket.dependencies
paket.lock
```

You can then run the application from within the folder as follows:

```bash
dotnet run --project src/MyApp
```

## I've never used Paket!
This is an opinioniated template, but of course feel free to remove it or fork this repository.

### Adding a package
```bash
cd src/MyApp
dotnet paket add <package name>
```
### Removing a package
```bash
cd src/MyApp
dotnet paket remove <package name>
```
### Safely updating all dependencies
```bash
dotnet paket update --keep-major
```