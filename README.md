# com.tsk.ide.vscode
Code editor integration for VSCode.

[![openupm](https://img.shields.io/npm/v/com.tsk.ide.vscode?label=openupm&registry_uri=https://package.openupm.com)](https://openupm.com/packages/com.tsk.ide.vscode/)

## Features
- Complete SDK support
- Auto Generation for omnisharp.json & .editorconfig
- useModernNet = true (predefined in omnisharp.json)
- Visual Studio's [Microsoft.Unity.Analyzers](https://github.com/microsoft/Microsoft.Unity.Analyzers) 

## API Compatibility Level Support
- .Net Framework 
  - Supports all Unity Versions(*)
- .Net Standard 
  - Supports 2022.1 and higher.

## Install via Package Manager

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
- Paste 1.3.0 into version
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
        "com.tsk.ide.vscode": "1.3.0"
    }
}
```
