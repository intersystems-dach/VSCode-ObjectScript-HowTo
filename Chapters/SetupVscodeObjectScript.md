# Setup Visual Studio Code for InterSystems ObjectScript

---

* [Install InterSystems Extensions](#install-intersystems-extensions)
* [Connect to a Server](#connect-to-a-server)
* [Open Namespace in Workspace via InterSystems Tools](#open-namespace-in-workspace-via-intersystems-tools)
* [Open Namespace in Workspace via Explorer](#open-namespace-in-workspace-via-explorer)

---

## Install InterSystems Extensions

Go to the Activity Bar on the far left-hand side and click on the  `Extensions` <img src = "https://i0.wp.com/www.phdata.io/wp-content/uploads/2021/06/VSCode-Extension-Icon-.png" tile = "Extensions Icon" width = "3%"/> tap.

Type in the search bar *InterSystems* and then install the [InterSystems ObjectScript Extension Pack](https://marketplace.visualstudio.com/items?itemName=intersystems-community.objectscript-pack) <img src = "https://intersystems-community.gallerycdn.vsassets.io/extensions/intersystems-community/objectscript-pack/1.0.3/1612388253024/Microsoft.VisualStudio.Services.Icons.Default" title = "OEP Icon" width = "3%"/>. This Extension pack includes:

* [InterSystems ObjectScript](https://marketplace.visualstudio.com/items?itemName=intersystems-community.vscode-objectscript): Adds InterSystems ObjectScript language support.
* [InterSystems Language Server](https://marketplace.visualstudio.com/items?itemName=intersystems.language-server): Adds InterSystems ObjectScript language server.
* [InterSystems Server Manager](https://marketplace.visualstudio.com/items?itemName=intersystems-community.servermanager): Define connections to InterSystems servers. Browse and manage those servers.

---

## Connect to a Server

* Open the `InterSystems Tools` <img src = "../imgs/InterSystemsToolsIcon.png" title = "InterSystemsToolsIcon" width = "3%"/> tap in the Activity Bar.
* You can see default configuartions under `All Servers`
* If you want to create a new Server connection click on the `+` button on the top and then fill in the connection properties:

  * *Name of new server definition*: Give your Connection a name.
  * *Optional Description*: A optional description for your server. Tap `Enter` to leave empty.
  * *Hostname or IP address of web server*: The Hostname or IP Address of your server.
  * *Port of web server*: The Port of the web server.
  * *Username*: The Username of your Iris user you want to connect from.
  * *Confirm connection type*: *http* or *https* connection type.

After successfully adding a new Server you can see the Server under `All Servers`.

> Tip: You can edit your Server Properties under: `...` in the top right corner > Edit Settings > InterSystems: Servers > Edit in settings.json

---

## Open Namespace in Workspace via InterSystems Tools

* Open the `InterSystems Tools` <img src = "../imgs/InterSystemsToolsIcon.png" title = "InterSystemsToolsIcon" width = "3%"/> tap in the Activity Bar.
* Choose a Server and click on it.
  * If the connection is succesfully you will the a new directory named *Namespaces*.
  * If the connection failed you will see *Unavailable at \<current-time\>*.
* Choose a namespace.
  * Click on the *eye-icon* next to your namespace to view the namespace in your workspace.
  * Click on the *pen-icon* next to your namespace to edit the namespace in your workspace.

---

## Open Namespace in Workspace via Explorer

* Open the `Explorer` tap in the Activity Bar.
* Do a right-click and choose `Add Server Namespace to Workspace`.
* Now choose your Server or create a new one with the `+` in the top right corner of the dialog.
* Choose a Namespace.

---

[Next Chapter]()
[Overview](../README.md)
