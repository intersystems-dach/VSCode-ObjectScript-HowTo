# Visual Studio Code mit InterSystems ObjectScript nutzen

InterSystems ObjectScript ist eine Programmiersprache, die in InterSystems-Datenbanken wie InterSystems IRIS und Caché verwendet wird. Visual Studio Code (VSCode) ist ein beliebter Texteditor, der zum Schreiben und Bearbeiten von ObjectScript-Code verwendet werden kann.

---

* [InterSystems Extensions installieren](#intersystems-extensions-installieren)
* [ObjectScript Farbschema wählen](#objectscript-farbschema-wählen)
* [Zu einem Server verbinden](#zu-einem-server-verbinden)
* [Anmeldeinformationen speichern](#anmeldeinformationen-speichern)
* [Einen Namespace öffnen](#einen-namespace-öffnen)
  * [Einen Namespace mit InterSystems Tools öffnen](#einen-namespace-mit-intersystems-tools-öffnen)
  * [Einen Namespace mit dem Explorer öffnen](#einen-namespace-mit-dem-explorer-öffnen)
* [ObjectScript Code schreiben](#objectscript-code-schreiben)
* [SQLTools benutzen](#sqltools-benutzen)

---

## InterSystems Extensions installieren
Gehen Sie zur Activity Bar auf der linken Seite und klicken Sie auf `Extensions` <img src = "https://i0.wp.com/www.phdata.io/wp-content/uploads/2021/06/VSCode-Extension-Icon-.png" tile = "Extensions Icon" width = "3%"/>.

Geben Sie in die Suchleiste *InterSystems* ein und installieren Sie dann das [InterSystems ObjectScript Extension Pack](https://marketplace.visualstudio.com/items?itemName=intersystems-community.objectscript-pack) <img src = "https://intersystems-community.gallerycdn.vsassets.io/extensions/intersystems-community/objectscript-pack/1.0.3/1612388253024/Microsoft.VisualStudio.Services.Icons.Default" title = "OEP Icon" width = "3%"/>. Dieses Extension Pack enthält:

* [InterSystems ObjectScript](https://marketplace.visualstudio.com/items?itemName=intersystems-community.vscode-objectscript): Fügt Unterstützung für die Sprache InterSystems ObjectScript hinzu.
* [InterSystems Language Server](https://marketplace.visualstudio.com/items?itemName=intersystems.language-server): Fügt InterSystems ObjectScript language server hinzu.
* [InterSystems Server Manager](https://marketplace.visualstudio.com/items?itemName=intersystems-community.servermanager): Definieren Sie Verbindungen zu InterSystems-Servern. Durchsuchen und verwalten Sie diese Server.

---

## ObjectScript Farbschema wählen

Um eine korrekte Farbhervorhebung bei der Arbeit mit Objectscript zu gewährleisten, wählen Sie ein InterSystems Farbschema.

* Navigieren Sie zu `File > Preferences > Color Theme`
* Wählen Sie `InterSystems Default Dark` oder `InterSystems Default Light` aus.

---

## Zu einem Server verbinden

* Öffnen Sie `InterSystems Tools` <img src = "../imgs/InterSystemsToolsIcon.png" title = "InterSystemsToolsIcon" width = "3%"/> in der Activity Bar.
* Sie können die Standardkonfigurationen unter `All Servers` sehen.
* Wenn Sie eine neue Serververbindung erstellen möchten, klicken Sie oben auf die Schaltfläche `+` und geben Sie dann die Verbindungseigenschaften ein:

  * *Name of new server definition*: Geben Sie Ihrer Verbindung einen Namen.
  * *Optional Description*: Eine optionale Beschreibung für Ihren Server. Tippen Sie auf `Enter`, um es leer zu lassen.
  * *Hostname or IP address of web server*: Der Hostname oder die IP-Adresse Ihres Servers.
  * *Port of web server*: Der Port des Webservers.
  * *Username*: Der Benutzername Ihres IRIS-Benutzers, von dem aus Sie sich verbinden möchten.
  * *Confirm connection type*: *http* oder *https* Verbindungstyp.

Nach erfolgreichem Hinzufügen eines neuen Servers können Sie den Server unter `All Servers` sehen.

> Tipp: Sie können Ihre Servereigenschaften bearbeiten unter: `...` in der oberen rechten Ecke `> Edit Settings > InterSystems: Servers > Edit in settings.json`.

---

## Anmeldeinformationen speichern

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

## Einen Namespace öffnen

### Einen Namespace mit InterSystems Tools öffnen

* Open the `InterSystems Tools` <img src = "../imgs/InterSystemsToolsIcon.png" title = "InterSystemsToolsIcon" width = "3%"/> tap in the Activity Bar.
* Choose a Server and click on it.
  * If the connection is succesfully you will see a new directory named *Namespaces*.
  * If the connection failed you will see *Unavailable at \<current-time\>*.
* Choose a namespace.
  * Click on the *eye-icon* next to your namespace to view the namespace in your workspace.
  * Click on the *pen-icon* next to your namespace to edit the namespace in your workspace.

### Einen Namespace mit dem Explorer öffnen

* Open the `Explorer` tap in the Activity Bar.
* Do a right-click and choose `Add Server Namespace to Workspace`.
* Now choose your Server or create a new one with the `+` in the top right corner of the dialog.
* Choose a Namespace.

---

## ObjectScript Code schreiben

Once you have connected to a Namespace, you can begin writing ObjectScript code. Here are the basic steps for doing so:

* Create a new file with the `.cls` file extension (for example, `MyPackage.MyClass.cls`)
* Write your ObjectScript code in this file.
* The class will be compiled after you saved the file.

You can also create other file with the extension .mac, .inc etc.

---

## SQLTools benutzen

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

[Nächstes Kapitel](TipsForVsCode.md)

[Vorheriges Kapitel](GettingStartedWithVSCode.md)

[Überblick](../README.md)

von [Philipp B.](https://github.com/phil1436)
