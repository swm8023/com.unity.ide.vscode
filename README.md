# TSK VSCode Editor

[![openupm](https://img.shields.io/npm/v/com.tsk.ide.vscode?label=openupm&registry_uri=https://package.openupm.com)](https://openupm.com/packages/com.tsk.ide.vscode/)

Code editor integration for VSCode. **(2021.3+)**  

See [Changelog](https://github.com/Chizaruu/com.tsk.ide.vscode/wiki/CHANGELOG).

## Features

### Project SDK Support

This package provides project SDK support according to .Net 7 and .Net 6. This means that you can use the latest C# features and language features in your Unity projects.

### Auto Generation for omnisharp.json & .editorconfig

The com.tsk.ide.vscode package automatically generates omnisharp.json and .editorconfig files, saving you the time and effort of setting up these files manually.

These files are essential for configuring Visual Studio Code to work efficiently with Unity.

### Predefined Settings for omnisharp.json (useModernNet = true)

The package comes with predefined settings for omnisharp.json.

This feature enables the use of modern .NET features in your Unity projects, improving their overall performance and stability.

### Microsoft.Unity.Analyzers [![NuGet](https://img.shields.io/nuget/v/Microsoft.Unity.Analyzers.svg)](https://nuget.org/packages/Microsoft.Unity.Analyzers)

The package also includes support for the [Microsoft.Unity.Analyzers](https://github.com/microsoft/Microsoft.Unity.Analyzers) library which provides additional code analysis and validation tools for Unity projects.

## Prerequisites

1. Install both the .Net 7 and .Net 6 SDKs - <https://dotnet.microsoft.com/en-us/download>
2. **[Windows only]** Logout or restart Windows to allow changes to `%PATH%` to take effect.
3. **[macOS only]** To avoid seeing "Some projects have trouble loading. Please review the output for more details", make sure to install the latest stable [Mono](https://www.mono-project.com/download/) release.
    - Note: This version of Mono, which is installed into your system, will not interfere with the version of MonoDevelop that is installed by Unity.
4. Install the C# extension from the VS Code Marketplace.
5. Install Build Tools for Visual Studio (Windows only)

The C# extension no longer ships with Microsoft Build Tools so they must be installed manually.

- Download the [Build Tools for Visual Studio 2022](https://visualstudio.microsoft.com/downloads/#build-tools-for-visual-studio-2022).
- Install the .NET desktop build tools workload. No other components are required.

## Install via Package Manager

### Unity

- Open Window/Package Manager
- Click +
- Select Add package from git URL
- Paste `https://github.com/Chizaruu/com.tsk.ide.vscode.git#upm` into URL
- Click Add

### OpenUPM

Please follow the instrustions:

- Open Edit/Project Settings/Package Manager
- Add a new Scoped Registry (or edit the existing OpenUPM entry)

```text
  Name: package.openupm.com
  URL: https://package.openupm.com
  Scope(s): com.tsk.ide.vscode
```

- Click Save (or Apply)
- Open Window/Package Manager
- Click +
- Select Add package by name... or Add package from git URL...
- Paste com.tsk.ide.vscode into name
- Paste 1.3.4 into version
- Click Add

Alternatively, merge the snippet to Packages/manifest.json

```json
{
    "scopedRegistries": [
        {
            "name": "package.openupm.com",
            "url": "https://package.openupm.com",
            "scopes": [
                "com.tsk.ide.vscode"
            ]
        }
    ],
    "dependencies": {
        "com.tsk.ide.vscode": "1.3.4"
    }
}
```

## Contributing

Thank you for considering contributing to the com.tsk.ide.vscode package! To contribute, please follow these guidelines:

- Create a new branch for your changes.
- Discuss your changes by creating a new issue in the repository before starting work.
- Follow the existing coding conventions and style.
- Provide a clear description of your changes in your pull request.
- Submit your pull request to the default branch.

We appreciate all contributions to com.tsk.ide.vscode!
