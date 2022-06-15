# Steps to Publish your own VS Extension

1. Create publisher on the [Marketplace management portal](https://aka.ms/vsmarketplace-manage)
1. Install `tfx` command line tool
    
    ```bash
    npm install -g tfx-cli
    ```
    
1. Navigate to the directory containing the `vss-extension.json`
1. Generate the `.vsix` file through `tfx extension create`
    
    ```bash
    > tfx extension create --rev-version
    
    TFS Cross Platform Command Line Interface v0.11.0
    Copyright Microsoft Corporation
    
    === Completed operation: create extension ===
     - VSIX: /mnt/c/Users/jinle/Documents/Tools/ADO-Decorator-Demo/Build/Pre/Jinle-SandboxExtensions.jinlesampledecoratorspre-1.0.0.vsix
     - Extension ID: jinlesampledecoratorspre
     - Extension Version: 1.0.0
     - Publisher: Jinle-SandboxExtensions
    ```
    
1. Upload the extension via the [Marketplace management portal](https://aka.ms/vsmarketplace-manage) or through `tfx extension publish`
1. Share your extension with your ADO Organization
1. Install the extension on your ADO Organization
    1. Organization Settings
        1. Manage Extensions
            1. Shared
                1. Install Extension

# Contribute
TODO: Explain how other users and developers can contribute to make your code better. 

If you want to learn more about creating good readme files then refer the following [guidelines](https://docs.microsoft.com/en-us/azure/devops/repos/git/create-a-readme?view=azure-devops). You can also seek inspiration from the below readme files:
- [ASP.NET Core](https://github.com/aspnet/Home)
- [Visual Studio Code](https://github.com/Microsoft/vscode)
- [Chakra Core](https://github.com/Microsoft/ChakraCore)