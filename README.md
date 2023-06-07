# Code Analyzer Tool Action
This repository hosts an action that installs and runs a custom code analyzer tool for .NET projects.

The code analyzer tool is a self-developed solution that performs analysis on project code. For more details about the tool, please refer to the repository in our organization.

When executed, this action will first install the .NET SDK (version 7.0) required for installing and running the dotnet tool.
Next, it will proceed with installing the dotnet tool itself, which is available as a NuGet package on Nuget.org.
Finally, the action will run the code analyzer tool.

The purpose of this action is to seamlessly integrate it into a workflow, facilitating code analysis functionalities.

Example usage in a workflow:
```yaml
name: Analyse the code
on: [push]
        
jobs:
    run-code-analyzer-tool:
        runs-on: ubuntu-latest
        steps:
            - name: Checkout the code
              uses: actions/checkout@v3.5.2
            - name: Run Code Analyzer Tool
              uses: CodeAnalyzerIS/code-analyzer-tool-action@v2.0.0
```
