# Using Visual Studio Code with InterSystems ObjectScript

InterSystems ObjectScript is a programming language that is used in InterSystems databases such as InterSystems IRIS and Caché. Visual Studio Code (VSCode) is a popular text editor that can be used to write and edit ObjectScript code.

---

* [Install InterSystems Extensions](#install-intersystems-extensions)
* [Set ObjectScript Color Theme](#set-objectscript-color-theme)
* [Connect to a Server](#connect-to-a-server)
* [Open a Namespace via InterSystems Tools](#open-a-namespace-via-intersystems-tools)
* [Open a Namespace via the Explorer](#open-a-namespace-via-the-explorer)
* [Writing ObjectScript Code](#writing-objectscript-code)

---

## Install InterSystems Extensions

Go to the Activity Bar on the far left-hand side and click on the  `Extensions` <img src = "https://i0.wp.com/www.phdata.io/wp-content/uploads/2021/06/VSCode-Extension-Icon-.png" tile = "Extensions Icon" width = "3%"/> tap.

Type in the search bar *InterSystems* and then install the [InterSystems ObjectScript Extension Pack](https://marketplace.visualstudio.com/items?itemName=intersystems-community.objectscript-pack) <img src = "https://intersystems-community.gallerycdn.vsassets.io/extensions/intersystems-community/objectscript-pack/1.0.3/1612388253024/Microsoft.VisualStudio.Services.Icons.Default" title = "OEP Icon" width = "3%"/>. This Extension pack includes:

* [InterSystems ObjectScript](https://marketplace.visualstudio.com/items?itemName=intersystems-community.vscode-objectscript): Adds InterSystems ObjectScript language support.
* [InterSystems Language Server](https://marketplace.visualstudio.com/items?itemName=intersystems.language-server): Adds InterSystems ObjectScript language server.
* [InterSystems Server Manager](https://marketplace.visualstudio.com/items?itemName=intersystems-community.servermanager): Define connections to InterSystems servers. Browse and manage those servers.

---

## Set ObjectScript Color Theme

To provide correct color highlighting when working with Objectscript choose a InterSystems Color Theme.

* Open the `Manage` <img src = "../imgs/ManageIcon.png" title = "InterSystemsToolsIcon" width = "3%"/> tap in the Activity Bar.
* Select `Color Theme`.
* Choose `InterSystems Default Dark` or `InterSystems Default Light`.

---

## Connect to a Server

* Open the `InterSystems Tools` <img src = "../imgs/InterSystemsToolsIcon.png" title = "InterSystemsToolsIcon" width = "3%"/> tap in the Activity Bar.
* You can see default configuartions under `All Servers`
* If you want to create a new Server connection click on the `+` button in the top and then fill in the connection properties:

  * *Name of new server definition*: Give your Connection a name.
  * *Optional Description*: A optional description for your server. Tap `Enter` to leave empty.
  * *Hostname or IP address of web server*: The Hostname or IP Address of your server.
  * *Port of web server*: The Port of the web server.
  * *Username*: The Username of your Iris user you want to connect from.
  * *Confirm connection type*: *http* or *https* connection type.

After successfully adding a new Server you can see the Server under `All Servers`.

> Tip: You can edit your Server Properties under: `...` in the top right corner `> Edit Settings > InterSystems: Servers > Edit in settings.json`.

---

## Open a Namespace via InterSystems Tools

* Open the `InterSystems Tools` <img src = "../imgs/InterSystemsToolsIcon.png" title = "InterSystemsToolsIcon" width = "3%"/> tap in the Activity Bar.
* Choose a Server and click on it.
  * If the connection is succesfully you will see a new directory named *Namespaces*.
  * If the connection failed you will see *Unavailable at \<current-time\>*.
* Choose a namespace.
  * Click on the *eye-icon* next to your namespace to view the namespace in your workspace.
  * Click on the *pen-icon* next to your namespace to edit the namespace in your workspace.

---

## Open a Namespace via the Explorer

* Open the `Explorer` tap in the Activity Bar.
* Do a right-click and choose `Add Server Namespace to Workspace`.
* Now choose your Server or create a new one with the `+` in the top right corner of the dialog.
* Choose a Namespace.

---

## Writing ObjectScript Code

Once you have connected to a Namespace, you can begin writing ObjectScript code. Here are the basic steps for doing so:

* Create a new file with the `.cls` file extension (for example, `MyPackage.MyClass.cls`)
* Write your ObjectScript code in this file.
* The class will be compiled after you saved the file.

You can also create other file with the extension .mac, .inc etc.

---

[Next Chapter](../README.md)

[Overview](../README.md)