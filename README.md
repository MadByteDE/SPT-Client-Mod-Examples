## SPT client mod examples

A template/example project for creating SPT client mods on Linux.

## Prerequisites

- **.NET 9.x SDK**
- **VSCode / VSCodium**

## Usage as template for a new project

#### 1. Clone the repository

    git clone https://github.com/MadByteDE/SPT-Client-Mod-Examples.git

#### 2. Edit the `GameDir` property in the `*.csproj` file

- Set it to the SPT install directory

> [!NOTE]
> <span style="color:lightblue">By default we assume the project directory to be located in a sub-directory of the game directory e.g. `../development/SPTClientModExamples/`</span>

#### 3. Replace all occurrences of `SPTClientModExamples` in the project
#### 4. Change the `AUTHOR` in `Plugin.cs`
#### 5. Generate a new GUID and replace the `ProjectGuid` in the `*.csproj` file
#### 6. Set optional attributes in `Properties/AssemblyInfo.cs`

## Building

To build the project, either use `CTRL+SHIFT+B` and selected a pre-defined task **OR** run:

```bash
    dotnet build --configuration Release # to build using the 'Release' config
    dotnet build --configuration Debug # to build using the 'Debug' config
```