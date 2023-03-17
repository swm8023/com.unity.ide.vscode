# com.tsk.ide.vscode
Code editor integration for VSCode.

[![openupm](https://img.shields.io/npm/v/com.tsk.ide.vscode?label=openupm&registry_uri=https://package.openupm.com)](https://openupm.com/packages/com.tsk.ide.vscode/)

## Install via Package Manager

Please follow the instrustions:

- Open Edit/Project Settings/Package Manager
- Add a new Scoped Registry (or edit the existing OpenUPM entry)
```text
  Name: package.openupm.com
  URL: https://package.openupm.com
```
- Click Save (or Apply)
- Open Window/Package Manager
- Click +
- Select Add package by name... or Add package from git URL...
- Paste com.tsk.ide.vscode into name
- Paste 1.2.6 into version
- Click Add

Alternatively, merge the snippet to Packages/manifest.json
```json
{
    "scopedRegistries": [
        {
            "name": "package.openupm.com",
            "url": "https://package.openupm.com",
            "scopes": []
        }
    ],
    "dependencies": {
        "com.tsk.ide.vscode": "1.2.6"
    }
}
```
