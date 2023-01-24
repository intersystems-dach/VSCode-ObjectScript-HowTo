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

Jedes Mal, wenn Sie Visual Studio Code schließen und erneut öffnen, werden Sie aufgefordert, sich mit Ihren Anmeldeinformationen anzumelden. Um dies zu vermeiden, können Sie Ihre Anmeldeinformationen speichern:

* Benutzernamen speichern:
  * In dem [Command Palette](KeyboardShortcuts.md#command-palette) schreibe *Preferences: Open User Settings (JSON)*. Hier sehen Sie Ihre Serververbindung im JSON-Format.
  * Wählen Sie den Server aus, dem Sie Ihren Benutzernamen hinzufügen möchten, und fügen Sie eine Eigenschaft namens *username* hinzu.

Beispiel:

````json
"default~iris": {
         "webServer": {
            ...
         },
         "username":"<your-username>",
         "description": "Connection to local InterSystems IRIS™ installed with default settings."
      }
````

* Passwort speichern
  * Wenn Sie Visual Studio Code das nächste mal öffnen, werden Sie zu einem Dialogfeld aufgefordert und nach einem Passwort gefragt
  * Geben Sie Ihr Passwort ein
  * Klicken Sie auf die *Schlüssel*-Schaltfläche in der oberen rechten Ecke des Dialogs, um das Passwort zu speichern
* Passwort löschen
  * Navigieren Sie zu *Accounts* in der Activity Bar
  * Wählen Sie Ihren Benutzer aus
  * Wählen Sie `Sign Out`
  * Wählen Sie `Delete` wenn Sie aufgefordert werden, das Passwort zu löschen

---

## Einen Namespace öffnen

### Einen Namespace mit InterSystems Tools öffnen

* Öffnen Sie `InterSystems Tools` <img src = "../imgs/InterSystemsToolsIcon.png" title = "InterSystemsToolsIcon" width = "3%"/> in der Activity Bar.
* Wählen Sie einen Server und klicken Sie darauf.
  * Wenn die Verbindung erfolgreich ist, sehen Sie ein neues Verzeichnis namens *Namespaces*.
  * Wenn die Verbindung fehlgeschlagen ist, sehen Sie *Unavailable at \<current-time\>*.
* Wählen Sie einen Namespace.
  * Klicken Sie auf das *Augen-Symbol* neben Ihrem Namespace, um den Namespace in Ihrem Workspace anzuzeigen.
  * Klicken Sie auf das *Stift-Symbol* neben Ihrem Namespace, um den Namespace in Ihrem Workspace zu bearbeiten.

### Einen Namespace mit dem Explorer öffnen

* Öffnen Sie den `Explorer` in der Activity Bar.
* Machen Sie einen Rechtsklick und wählen Sie `Add Server Namespace to Workspace`.
* Wählen Sie nun Ihren Server aus oder erstellen Sie einen neuen mit dem `+` Knopf in der oberen rechten Ecke des Dialogs.
* Wähle Sie einen Namespace.

---

## ObjectScript Code schreiben

Nachdem Sie eine Verbindung zu einem Namespace hergestellt haben, können Sie mit dem Schreiben von ObjectScript-Code beginnen. Hier sind die grundlegenden Schritte dafür:

* Erstellen Sie eine neue Datei mit der Dateiendung `.cls`.(z.B.  `MyPackage.MyClass.cls`)
* Schreiben Sie Ihren ObjectScript-Code in diese Datei.
* Die Klasse wird kompiliert, nachdem Sie die Datei gespeichert haben.

Sie können auch andere Dateien mit der Endung .mac, .inc usw. erstellen.

---

## SQLTools benutzen

Wenn Sie einen Blick in Ihre Datenbank werfen möchten, ohne Visual Studio Code zu verlassen, können Sie die SQLTools-Extension verwenden.

* Installieren Sie die [SQLTools](https://marketplace.visualstudio.com/items?itemName=mtxr.sqltools) Extension
* Installieren Sie die [SQLTools InterSystems IRIS](https://marketplace.visualstudio.com/items?itemName=intersystems-community.sqltools-intersystems-driver) Extension
* Navigieren Sie zum Tap SQLTools <img src ="https://raw.githubusercontent.com/intersystems-community/sqltools-intersystems-driver/master/docs/assets/img/activitybar.png" title = "SQLTools icon"> in der Activity Bar und wählen Sie `Add New Connection`
* Wählen Sie *InterSystems IRIS* und füllen Sie die Verbindungseigenschaften aus
* Wählen Sie `Connect Now` und Sie sehen eine neue Verbindung unter *Connections*
* Jetzt können Sie eine neue SQL-Datei erstellen und die Abfrage auf Ihrer Verbindung mit `Run on active connection` ausführen
**ODER**
* Durchsuchen Sie Ihre Tabellen und Views, indem Sie die Verbindung aufklappen, und zeigen Sie dann die Tabelle oder Ansicht an, indem Sie auf das Lupensymbol klicken.

---

[Nächstes Kapitel](TipsForVsCode.md)

[Vorheriges Kapitel](GettingStartedWithVSCode.md)

[Überblick](../README.md)

von [Philipp B.](https://github.com/phil1436)
