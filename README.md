| Latest Version | Azure Pipelines | Test Status | PowerShell Gallery | Github Release | Issues | License | Forks |
|-----------------|-----------------|----------------|----------------|----------------|----------------|----------------|----------------|
| ![Latest Version](https://img.shields.io/github/v/tag/SchemaModule/PowerShell)
| ![Azure Pipelines Build Status](https://img.shields.io/azure-devops/build/patton-tech/c31a2770-9aee-4799-a078-eee0dc12cbf4/5)
| ![Azure Build Test Results](https://img.shields.io/azure-devops/tests/patton-tech/c31a2770-9aee-4799-a078-eee0dc12cbf4/5)
| ![Powershell Gallery](https://img.shields.io/powershellgallery/dt/SchemaModule)
| ![Github Release](https://img.shields.io/github/downloads/SchemaModule/PowerShell/total)
| [![GitHub issues](https://img.shields.io/github/issues/SchemaModule/PowerShell)](https://github.com/SchemaModule/PowerShell/issues)
| [![GitHub forks](https://img.shields.io/github/forks/SchemaModule/PowerShell)](https://github.com/SchemaModule/PowerShell/network)
| [![GitHub license](https://img.shields.io/github/license/SchemaModule/PowerShell)](https://github.com/SchemaModule/PowerShell/blob/master/LICENSE)

# About

The SchemaModule project grew out of a need to create PowerShell objects from a well-defined JSON schema. The functions
included with this module should help a developer leverage objects and properties to create objects on-demand. The
intended use-case is for this module to be used inside a script or other module to faciliate the creation of objects and
ultimately validation.

# Function Documentation
Below is the list of current functions and their documentation.

## [Get-SchemaArray](docs/Get-SchemaArray.md)
This function returns the object from an array within the Json Schema.

## [Get-SchemaDocument](docs/Get-SchemaDocument.md)
This function will return a PowerShell object of the input Schema.

## [Get-SchemaObject](docs/Get-SchemaObject.md)
This function returns an object from the Json Schema.

## [Get-SchemaProperty](docs/Get-SchemaProperty.md)
This function returns one ore more properties from a Json Schema object.

### Documentation

This project uses [PlatyPS](https://github.com/PowerShell/platyPS) for framing and updating the help files and external help used by the functions.

### Automation

A few things within each module are automated by [psake](https://github.com/psake/psake) such as the functions that are exported, as well as the README file for each module.

### Syntax Checking

[PSScriptAnalyzer](https://github.com/PowerShell/PSScriptAnalyzer) is used to check the code against a set of [standards](https://github.com/PowerShell/PSScriptAnalyzer/blob/master/RuleDocumentation/README.md), this ensures that the code works as expected when ran.