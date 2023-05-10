# Code Analyzer Tool Action
This repository contains the action to install and run a self-made code analyzer dotnet tool

The code analyzer is a selfmade tool that analyses project code. To see what the code analyzer tool is, check out the repo in our organisation.

This action will first install the .NET SDK (7.0) that is used to install and run the dotnet tool  
Afterwards it will perform a step to install the dotnet tool which is a Nuget package from Nuget.org  
As last step it will run the analyzer tool.

The purpose of this action is to integrate it in a workflow for analysation purposes.
