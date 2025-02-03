## SPT client mod examples

This repository can be used as a template for developing / building SPT client mod projects on Linux.

It's a fork of Jehree's [SPTClientModExamples](https://github.com/Jehree/SPTClientModExamples) repo.

## Prerequisites

- .NET 9.x SDK
- VSCode / VSCodium

## Setting up the environment

**SPT development directory**

For simplicity, it's recommended to create a new `development` directory inside your installation of SPTarkov, e.g `~/Games/escape-from-tarkov/drive_c/SPTarkov`. 

This will make it easier to reference modules in the game directory like this:

```c#
    <Reference Include="UnityEngine">
      <HintPath>..\..\EscapeFromTarkov_Data\Managed\UnityEngine.dll</HintPath>
    </Reference>
```


## Usage as template for new projects

1. Clone this repo
2. Rename the following from `SPTClientModExamples` to your new mod name:
    * The base project directory
    * **.csproj** file
3. Open the **.csproj** file with a text editor, search for `SPTClientModExamples` and replace it with your new mod name
4. Press `CTRL + Shift + F`, click Replace in Files
    * in **Find** field, enter: `SPTClientModExamples`
    * in **Replace** field, enter your new mod name
    * click `Replace All` in bottom right, click `yes` if prompted

## Building

To build the project, use:

```bash
    dotnet build --configuration Release # to build using the Release config
    dotnet build --configuration Debug # to build using the Debug config
```