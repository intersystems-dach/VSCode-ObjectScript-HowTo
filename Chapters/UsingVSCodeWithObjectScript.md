# Using Visual Studio Code with InterSystems ObjectScript

InterSystems ObjectScript is a programming language that is used in InterSystems databases such as InterSystems IRIS and Caché. Visual Studio Code (VSCode) is a popular text editor that can be used to write and edit ObjectScript code.

---

* [Install InterSystems Extensions](#install-intersystems-extensions)
* [Set ObjectScript Color Theme](#set-objectscript-color-theme)
* [Connect to a Server](#connect-to-a-server)
* [Store Credentials](#store-credentials)
* [Open a Namespace](#open-a-namespace)
  * [Open a Namespace via InterSystems Tools](#open-a-namespace-via-intersystems-tools)
  * [Open a Namespace via the Explorer](#open-a-namespace-via-the-explorer)
* [Writing ObjectScript Code](#writing-objectscript-code)
* [Use SQLTools](#use-sqltools)

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

* Navigate to `File > Preferences > Color Theme`
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

## Store Credentials

Everytime you close Visual Studio Code and reopen it, it will prompt you a message with

* Store Username:
  * In the [Command Palette](KeyboardShortcuts.md#command-palette) type *Preferences: Open User Settings (JSON)*. Here you can see your server connection in a JSON format.
  * Choose the server you want to add your username and add a property called *username*

Example:

````json
"default~iris": {
         "webServer": {
            ...
         },
         "username":"<your-username>",
         "description": "Connection to local InterSystems IRIS™ installed with default settings."
      }
````

* Store password
  * Next time you open Visual Studio code, it will prompt you a dialog and ask for a password
  * Type in your password
  * Click on the *key* button in the top right corner of the dialog to store the password
* Delete password
  * Navigate to *Accounts* in the Activity Bar
  * Select your user
  * Click on `Sign Out`
  * select `Delete` when asked to delete password

---

## Open a Namespace

### Open a Namespace via InterSystems Tools

* Open the `InterSystems Tools` <img src = "../imgs/InterSystemsToolsIcon.png" title = "InterSystemsToolsIcon" width = "3%"/> tap in the Activity Bar.
* Choose a Server and click on it.
  * If the connection is succesfully you will see a new directory named *Namespaces*.
  * If the connection failed you will see *Unavailable at \<current-time\>*.
* Choose a namespace.
  * Click on the *eye-icon* next to your namespace to view the namespace in your workspace.
  * Click on the *pen-icon* next to your namespace to edit the namespace in your workspace.

### Open a Namespace via the Explorer

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

## Use SQLTools

When you want to have a look inside your database without leaving Visual Studio Code, you can use the SQLTools extension.

* Install the [SQLTools](https://marketplace.visualstudio.com/items?itemName=mtxr.sqltools) extension
* Install the [SQLTools InterSystems IRIS](https://marketplace.visualstudio.com/items?itemName=intersystems-community.sqltools-intersystems-driver)
* Navigate to the SQLTools tap <img src ="https://raw.githubusercontent.com/intersystems-community/sqltools-intersystems-driver/master/docs/assets/img/activitybar.png" title = "SQLTools icon"> in the Activity Bar and choose `Add New Connection`
* Choose *InterSystems IRIS* and fill out the connection properties
* Choose `Connect Now` and you will see a new connection under *Connections*
* Now you can create a new SQl file and run the Query on your connection with `Run on active connection`
**OR**
* Browse through your tables and views, by unfolding the connection, and then view the table or view by clicking on the magnifyingglasses icon.

---

[Next Chapter](TipsForVsCode.md)

[Previous Chapter](GettingStartedWithVSCode.md)

[Overview](../README.md)

by [Philipp B.](https://github.com/phil1436)
