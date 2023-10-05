# Tipps zur Verwendung von Visual Studio Code

Hier sind ein paar Tipps, die Ihnen dabei helfen sollen, Visual Studio Code optimal zu nutzen.

---

## Editor Playground

Wenn Sie gerade erst mit Visual Studio Code beginnen, können Sie den _Editor Playground_ unter `Help > Editor Playground` ausprobieren. Hier erfahren Sie, wie Sie einige der leistungsstarken [Codebearbeitungsfunktionen](https://code.visualstudio.com/docs/editor/codebasics) verwenden.

## Command Palette

Die Command Palette ist ein leistungsstarkes Tool, mit dem Sie schnell und einfach auf fast alle Funktionen oder Befehle in Visual Studio Code zugreifen können. Hier können Sie auch schnell die Tastenbelegungen nachschlagen, falls Sie eine vergessen haben. Um die Command Palette zu öffnen, drücken Sie `Ctrl + Shift + P` (Windows/Linux) oder `Cmd + Shift + P` (macOS).

## Verwenden Sie das integrierte Terminal

Visual Studio Code enthält ein integriertes Terminal, mit dem Sie Befehlszeilentools wie git und npm ausführen können. Um das Terminal zu öffnen, drücken Sie `Ctrl + Shift + Ö` (Windows/Linux) oder `Cmd + Shift + Ö` (macOS).

## Verwenden Sie Codeschnipsel

Visual Studio Code enthält eine Vielzahl integrierter Codeausschnitte, mit denen Sie beim Schreiben von Code Zeit sparen können. Sie können zum Beispiel "for" eingeben und dann `Ctrl + Space` (Windows/Linux) oder `Cmd + Space` (macOS) drücken, um schnell eine for-Schleife zu erstellen. Sie können auch Ihre eigenen benutzerdefinierten Codeausschnitte erstellen, indem Sie zu `File > Preferences > Configure User Snippets` gehen.

## Passen Sie das Farbschema an

Visual Studio Code enthält mehrere integrierte Farbschema, mit denen Sie das Erscheinungsbild des Editors anpassen können. Sie können das Farbschema ändern, indem Sie zu `File > Preferences > Color Theme` gehen. Um weitere Farbschemen zu finden, können Sie den Marktplatz verwenden.

## Extensions benutzen

Visual Studio Code verfügt über ein riesiges Ökosystem von [Extensions](https://marketplace.visualstudio.com/), die dem Editor neue Features und Funktionen hinzufügen. Sie können Erweiterungen suchen und installieren, indem Sie zu `File > Extensions` gehen. Sehen Sie sich auch [Die wichtigestens Visual Studio Code Extensions](EssentialExtensions.md) an.

## Lernen Sie die Tastenkombinationen

Visual Studio Code verfügt über eine große Anzahl von Tastenkombinationen, mit denen Sie schneller und effizienter arbeiten können. Sie können die vollständige Liste der Tastenkombinationen anzeigen, indem Sie zu `File > Preferences > Keyboard Shortcuts` gehen, wo Sie auch die Tastaturkürzel anpassen können. Sehen Sie sich auch [Tastenkombinationen für Visual Studio Code](KeyboardShortcuts.md) an.

## Beim Speichern formatieren

Es ist nicht immer einfach, Ihren Code manuell in einem gut lesbaren Zustand zu halten. Glücklicherweise bietet Visual Studio Code einen Formatierer für fast jede Sprache. Um Ihren Code gleichzeitig mit dem Speichern zu formatieren, können Sie die Funktion `Format On Save` aktivieren:

-   Öffnen Sie die Einstellungen unter `File > Preferences > Settings` oder über `Strg + ,`
-   Tippen Sie _Format On Save_
-   Aktivieren Sie das Kästchen für `Editor: Format On Save`

## Sticky Scroll

Wenn Sie Code mit langen Klassen und Methoden arbeiten, die über die vertikale Größe Ihres Bildschirms hinausgehen, kann es schwierig sein, den Überblick zu behalten, in welchem ​​Bereich Sie arbeiten. Visual Studio Code bietet jetzt eine Funktion, um einen besseren Überblick über Ihren Code zu haben: **Sticky Scroll**

-   Öffnen Sie die Einstellungen unter `File > Preferences > Settings` oder über `Strg + ,`
-   Tippen Sie _Sticky Scroll_
-   Aktivieren Sie das Kästchen für `Editor › Sticky Scroll: Enabled`

## Passen Sie die Einstellungen an

Mit Visual Studio Code können Sie verschiedene Einstellungen anpassen, z. B. die Schriftgröße, die Tabgröße und die Anzahl der für Einzüge verwendeten Leerzeichen. Sie können auf diese Einstellungen zugreifen, indem Sie zu `File > Preferences > Settings` gehen. Hier können Sie die Datei settings.json bearbeiten, die alle Ihre Visual Studio Code-Einstellungen enthält.

Hier finden Sie nützliche Einstellungen sowie

-   `editor.renderWhitespace`: Rendern Sie Leerzeichen in Ihrem Code für eine bessere Sichtbarkeit.
-   `editor.tabSize`: Passen Sie die Größe des Tabs an
-   `editor.fontSize` : Passen Sie die Größe der Schriftart an

## Settings Sync

Sie können Ihre Einstellungen, Tastenkombinationen und Extensions auf allen Geräten synchronisieren mit _[Settings Sync](https://code.visualstudio.com/docs/editor/settings-sync)_. Melden Sie sich einfach mit Ihrem GitHub- oder Microsoft-Benutzer an.

## Verwenden Sie Code-Navigationsfunktionen

Visual Studio Code enthält Features wie Go to Definition, Find All References und Peek Definition, die beim Navigieren durch Ihre Codebasis nützlich sein können.

## FiraCode Schriftart

Installieren Sie die [FiraCode Schriftart](https://github.com/tonsky/FiraCode) um Symbole, die mit mehreren Zeichen kodiert sind, wie `>=` oder `!=`, zu einem Zeichen anzeigen zu lassen.

## Erstellen Sie Ihre eigenen Extensions

Visual Studio Code bietet eine Vielzahl von Extensions und es gibt fast für alles eine Extension. Aber manchmal stoßen Sie auf ein Problem, bei dem keine Extensions vorhanden ist, um dieses Problem zu lösen. Das könnte der Punkt sein, an dem Sie beginnen [Ihre eigenen Erweiterungen erstellen](https://code.visualstudio.com/api/get-started/your-first-extension).

---

[Nächstes Kapitel](KeyboardShortcuts.md)

[Vorheriges Kapitel](UsingVSCodeWithObjectScript.md)

[Überblick](../README.md)

von [Philipp B.](https://github.com/phil1436)
