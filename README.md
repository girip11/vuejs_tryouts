# Fastapi VueJS Web Application

## IDE

**VSCode** is used as the IDE for this project.

- [VSCode on linux](https://code.visualstudio.com/docs/setup/linux)
- [VSCode on Mac](https://code.visualstudio.com/docs/setup/mac)

All required vscode extensions for frontend and backend are available in the `extensions.json` located inside `.vscode` in the respective folders.

## Installing extensions

**NOTE**: Few extensions might not work out of the box. Ex: pgformatter, shell-format etc.

### Installing extensions via commandline(recommended)

Get the list of all the extensions from `.vscode/extensions.json` and then you could use the following command to install the extensions `code --install-extension <extension_name>`.

Make sure that vscode is in the `PATH` for the above command to work.

### Installing extensions via UI

**NOTE**: If you try to open a workspace file without installing the project dependencies, then VSCode could raise few error events. So if you want to install extensions through UI(and you have to install one by one manually), then first setup the backend/frontend and then open the respective workspace in VSCode to install the extensions.

To install the recommended extensions, first open the workspace (**File -> Open workspace**) by opening either the `backend.code-workspace` or `frontend.code-workspace`. After the workspace is opened in VSCode, visit the extensions tab by clicking on the extensions icon on the left pane(hovering over the icons will reveal the name of the tab that the icon will open).

In the extensions tab, type `@recommended:workspace`, so that all the extensions listed in the `.vscode/extensions.json` will be listed and you could install them.

## Project environment setup

Refer [Backend Application readme](backend/README.md) for setting up the backend project and [Frontend Application readme](frontend/README.md) for setting up the frontend project
