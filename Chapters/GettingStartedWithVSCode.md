# Erste Schritte mit Visual Studio Code

Visual Studio Code (VSCode) ist ein leichtgewichtiger und dennoch leistungsstarker Quellcode-Editor, der von Microsoft für Windows, Linux und macOS entwickelt wurde. Er verfügt über integrierte Unterstützung für Debugging, Quellcodekontrolle und Entwicklungsaufgaben wie Linting und Build. In dieser Dokumentation werden wir die Grundlagen der Verwendung von Visual Studio Code zum Schreiben, Debuggen und Verwalten Ihres Codes erläutern.

---

* [Install Visual Studio Code](#install-visual-studio-code)
* [Opening a project](#opening-a-project)
* [The Visual Studio Code interface](#the-visual-studio-code-interface)
* [Writing and editing code](#writing-and-editing-code)
* [Workspaces](#workspaces)
* [Settings](#settings)
* [Color Theme](#color-theme)
* [Debugging and testing](#debugging-and-testing)
* [Source Control](#source-control)

---

## Installiere Visual Studio Code

Bevor du anfangen kannst Visual Studio Code zu benutzen, musst du die passende Version für dein Betriebsystem [downloaden und installieren](https://code.visualstudio.com/download). Wenn die Installation abgeschlossen ist, kannst du Visual Studio Code starten, indem das Symbol auf deinem Desktop anklickst oder im Start Menü (Windows) oder Spotlight (macOS) nach "Visual Studio Code" suchst.

---

## Ein Projekt öffnen

Wenn du Visual Studio Code das erste mal startest, wird dir ein Fenster mit *Open Folder* angezeigt. Hiermit kannst du ein bereits exestierendes Projekt öffnen oder ein neues Projekt erstellen, indem du nach `File > New Folder` navigierst und dann den neuen Ordner auswählst. Wenn du einen Ordner geöffnet hast, kannst du anfangen Datein zu deinem Projekt hinzuzufügen und bearbeiten.

---

## Die Visual Studio Code Oberfläche

Die Visual Studio Code Oberfläche teilt sich in ein paar Hauptbereiche auf:

<img src = "https://code.visualstudio.com/assets/api/ux-guidelines/examples/architecture-containers.png" tile = "VSCode Interface"/>

### Activity Bar

Die Activity Bar ist eine der Hauptnavigationsflächen in Visual Studio Code, die sich auf der linken Seite des Fensters befindet und Zugriff auf verschiedene Ansichten und Funktionen, wie den Datei-Explorer und die Debug-Konsole, bietet.

### Primary Sidebar

Hier werden die Inhalte der Activity Bar dargestellt.

### Secondary Sidebar

A secondary sidebar. You can drag items from other containers to here, to see more at a time.

### Editor

Here you will spend most of your time, writing and editing code.

### Panel

The Panel is an other area to view containers.

### Status Bar

Located at the bottom of the window, provides information and shortcuts for common actions.

---

## Code schreiben und editieren

Visual Studio Code has many powerful features for writing and editing code, including:

* **Syntax highlighting**: Visual Studio Code automatically recognizes the type of code you're working with and applies color coding to make it easier to read and write.
* **IntelliSense**: Visual Studio Code provides intelligent code completion and suggestions for many languages, making it easier to write code quickly and correctly.
* **Code snippets**: Visual Studio Code includes a large collection of code snippets that can be inserted into your code with a few keystrokes, saving you time and effort.

---

## Workspaces

Select `File > Open File / Open Folder` to open a file or a folder as a workspace.

### Add to current Workspace

Select `File > Add Folder to Workspace...` then select a folder to add to your current Workspace.

### Workspace speichern

So you dont have to open all your folders in your workspace everytime you open Visual Studio Code, you can save your Workspace as a file. Select `File > Save Workspace As...` and choose a destination and name for your workspace file. Afterwards a *.code-workspace* file was created. You can then open the workspace by just open the file or via `File > Open Workspace from File...`

---

## Einstellungen

Öffne die Einstellungen mit `File > Preferences > Settings`.

### User Einstellungen

When editing settings in the *User* tap all settings apply globally across all Visual Studio Code Workspaces.

### Workspace Einstellungen

When editing settings in the *Workspace* tap all settings applied only effects the current opened workspace.

---

## Farbe

You can customize the appearance of the Visual Studio Code interface to your needs. Navigate to `File > Preferences > Color Theme` there you can choose from a preinstalled Color Theme or install a new Color Theme with `+ Browse Additional Color Themes...`

---

## Debugging and testing

Visual Studio Code includes built-in support for debugging many languages, including JavaScript, TypeScript, and Python. To start debugging, you need to configure a "launch.json" file, which tells Visual Studio Code how to start and attach to your application. Once you have a launch configuration set up, you can start debugging by clicking the play button in the debug view or by pressing F5.

---

## Source Control

Visual Studio Code support source control systems like Git, SVN, and TFS. The source control icon will appear on the left sidebar once you open a folder that is a git repository, allowing you to see the changes, make commits and handle merge conflicts, among other functionalities.

---

These are just a few of the many features that Visual Studio Code has to offer. With its powerful editing capabilities, built-in support for debugging and testing, and integration with source control, Visual Studio Code is a great choice for a wide range of development tasks. As you become more familiar with the tool, you'll find that it can help you work more efficiently and effectively.

---

[Nächstes Kapitel](UsingVSCodeWithObjectScript.md)

[Überblick](../README.md)

von [Philipp B.](https://github.com/phil1436)
