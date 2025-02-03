## SPT client mod examples

This repository can be used as a template for developing / building SPT client mod projects on Linux.

It's a fork of Jehree's [SPTClientModExamples](https://github.com/Jehree/SPTClientModExamples) repo.

## Prerequisites

- .NET 9.x SDK
- VSCode / VSCodium

## Usage as template for a new project

1. Clone the repository
2. Replace all occurrences of `SPTClientModExamples` in the project
3. Change the `AUTHOR` in `Plugin.cs`
4. Generate a new GUID and replace the `ProjectGuid` in the *.csproj file
5. Add optional info in `Properties/AssemblyInfo.cs`

## Building

To build the project, either use `CTRL+SHIFT+B` and selected a pre-defined task **OR** run:

```bash
    dotnet build --configuration Release # to build using the 'Release' config
    dotnet build --configuration Debug # to build using the 'Debug' config
```