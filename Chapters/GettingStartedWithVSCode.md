# Erste Schritte mit Visual Studio Code

Visual Studio Code (VSCode) ist ein leichtgewichtiger und dennoch leistungsstarker Quellcode-Editor, der von Microsoft für Windows, Linux und macOS entwickelt wurde. Er verfügt über integrierte Unterstützung für Debugging, Quellcodekontrolle und Entwicklungsaufgaben wie Linting und Build. In dieser Dokumentation werden wir die Grundlagen der Verwendung von Visual Studio Code zum Schreiben, Debuggen und Verwalten Ihres Codes erläutern.

---

* [Installiere Visual Studio Code](#installiere-visual-studio-code)
* [Ein Projekt öffnen](#ein-projekt-öffnen)
* [Die Visual Studio Code Oberfläche](#die-visual-studio-code-oberfläche)
* [Code schreiben und editieren](#code-schreiben-und-editieren)
* [Workspaces](#workspaces)
* [Einstellungen](#einstellungen)
* [Farbeschema](#farbeschema)
* [Debuggen und Testen](#debuggen-und-testen)
* [Quellcodekontrolle](#quellcodekontrolle)

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

Eine zweite Seitenansicht. Hier können Inhalte von anderen Bereichen hineingezogen werden, um einen besseren Überblick zu haben.

### Editor

Hier kann man code schreiben und editieren.

### Panel

Das Panel ist eine andere Ansicht um Inhalt anzeigen zu lassen.

### Status Bar

Am unteren Rand des Fensters finden Sie Informationen und Kurzzugriffe für gängige Aktionen.

---

## Code schreiben und editieren

Visual Studio Code verfügt über viele leistungsstarke Funktionen zum Schreiben und Bearbeiten von Code, darunter:

* **Syntax highlighting**: Visual Studio Code erkennt automatisch die Art des Codes, mit dem Sie arbeiten, und wendet eine Farbcodierung an, um das Lesen und Schreiben zu erleichtern.
* **IntelliSense**: Visual Studio Code bietet intelligente Code-Vervollständigung und Vorschläge für viele Sprachen, die das schnelle und korrekte Schreiben von Code erleichtern.
* **Code snippets**: Visual Studio Code enthält eine große Sammlung von Codeschnipseln, die mit wenigen Tastendrücken in Ihren Code eingefügt werden können, wodurch Sie Zeit und Mühe sparen.

---

## Workspaces

Wählen Sie `File > Open File / Open Folder` um eine Datei oder Ordner als Workspace zu öffnen.

### Zum aktuellen Workspace hinzufügen

Wählen Sie `File > Add Folder to Workspace...` und wählen Sie dann einen Ordner aus, den Sie zu Ihrem aktuellen Workspace hinzufügen möchten.

### Workspace speichern

Damit Sie nicht jedes Mal alle Ordner in Ihrem Workspace öffnen müssen, wenn Sie Visual Studio Code öffnen, können Sie Ihren Arbeitsbereich als Datei speichern. Wählen Sie `File > Save Workspace As...` und wählen Sie ein Ziel und einen Namen für Ihre Workspacedatei. Anschließend wird eine *.code-workspace* Datei erstellt. Sie können den Workspace dann öffnen, indem Sie einfach die Datei öffnen oder über `File > Open Workspace from File...` die Datei auswählen.

---

## Einstellungen

Öffne die Einstellungen mit `File > Preferences > Settings`.

### User Einstellungen

Beim Bearbeiten von Einstellungen im *User* Tap gelten alle Einstellungen global für alle Visual Studio Code Workspaces.

### Workspace Einstellungen

Beim Bearbeiten von Einstellungen im *Workspace* Tap werden alle Einstellungen nur auf den aktuell geöffneten Workspace angewendet werden.

---

## Farbeschema

Sie können das Aussehen der Visual Studio Code-Oberfläche an Ihre Bedürfnisse anpassen. Navigieren Sie zu `File > Preferences > Color Theme`, dort können Sie aus einem vorinstallierten Farbeschema wählen oder mit `+ Browse Additional Color Themes...` ein neues Farbschema installieren.

---

## Debuggen und Testen

Visual Studio Code bietet integrierte Unterstützung für das Debugging vieler Sprachen, darunter JavaScript, TypeScript und Python. Um mit dem Debuggen zu beginnen, müssen Sie eine "launch.json"-Datei konfigurieren, die Visual Studio Code mitteilt, wie die Anwendung gestartet und angehängt werden soll. Sobald Sie eine Startkonfiguration eingerichtet haben, können Sie das Debuggen starten, indem Sie in der Debug-Ansicht auf die Schaltfläche "Play" klicken oder F5 drücken.

---

## Quellcodekontrolle

Visual Studio Code unterstützt Quellcodekontrollsysteme wie Git, SVN und TFS. Das Symbol für die Quellcodekontrolle wird in der linken Seitenleiste angezeigt, sobald Sie einen Ordner öffnen, der ein Git-Repository ist. So können Sie unter anderem die Änderungen sehen, Übertragungen vornehmen und Konflikte beim Zusammenführen behandeln.

---

Dies sind nur einige der vielen Funktionen, die Visual Studio Code zu bieten hat. Mit seinen leistungsstarken Bearbeitungsfunktionen, der integrierten Unterstützung für Debugging und Tests und der Integration in die Quellcodekontrolle ist Visual Studio Code eine hervorragende Wahl für eine Vielzahl von Entwicklungsaufgaben. Wenn Sie sich mit dem Tool vertraut machen, werden Sie feststellen, dass es Ihnen helfen kann, effizienter und effektiver zu arbeiten.

---

[Nächstes Kapitel](UsingVSCodeWithObjectScript.md)

[Überblick](../README.md)

von [Philipp B.](https://github.com/phil1436)
