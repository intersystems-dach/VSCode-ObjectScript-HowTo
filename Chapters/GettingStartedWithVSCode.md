# Getting Started with Visual Studio Code

Visual Studio Code (VSCode) is a lightweight yet powerful source code editor developed by Microsoft for Windows, Linux, and macOS. It comes with built-in support for debugging, source control, and development tasks such as linting and building. In this guide, we will walk through the basics of using Visual Studio Code to write, debug, and manage your code.

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

## Install Visual Studio Code

Before you can start using Visual Studio Code, you need to [download and install](https://code.visualstudio.com/download) the appropriate version for your operating system. Once the installation is complete, you can launch Visual Studio Code by double-clicking the icon on your desktop or by searching for "Visual Studio Code" in the start menu (on Windows) or spotlight (on macOS).

---

## Opening a project

When you first launch Visual Studio Code, you will be presented with an *Open Folder* dialog. You can use this to open an existing project, or you can create a new one by clicking `File > New Folder` and then selecting the new folder. Once you have a folder open, you can start adding and editing files within that folder.

---

## The Visual Studio Code interface

The Visual Studio Code interface is divided into a few key areas:

<img src = "https://code.visualstudio.com/assets/api/ux-guidelines/examples/architecture-containers.png" tile = "VSCode Interface"/>

### Activity Bar

The Activity Bar is a core navigation surface in Visual Studio Code located on the left side of the window, provides access to various views and features such as the file explorer and debug console.

### Primary Sidebar

Will open the content of a Activity Bar Item.

### Secondary Sidebar

A secondary sidebar. You can drag items from other containers to here, to see more at a time.

### Editor

Here you will spend most of your time, writing and editing code.

### Panel

The Panel is an other area to view containers.

### Status Bar

Located at the bottom of the window, provides information and shortcuts for common actions.

---

## Writing and editing code

Visual Studio Code has many powerful features for writing and editing code, including:

* **Syntax highlighting**: Visual Studio Code automatically recognizes the type of code you're working with and applies color coding to make it easier to read and write.
* **IntelliSense**: Visual Studio Code provides intelligent code completion and suggestions for many languages, making it easier to write code quickly and correctly.
* **Code snippets**: Visual Studio Code includes a large collection of code snippets that can be inserted into your code with a few keystrokes, saving you time and effort.

---

## Workspaces

Select `File > Open File / Open Folder` to open a file or a folder as a workspace.

### Add to current Workspace

Select `File > Add Folder to Workspace...` then select a folder to add to your current Workspace.

### Save Workspace

So you dont have to open all your folders in your workspace everytime you open Visual Studio Code, you can save your Workspace as a file. Select `File > Save Workspace As...` and choose a destination and name for your workspace file. Afterwards a *.code-workspace* file was created. You can then open the workspace by just open the file or via `File > Open Workspace from File...`

---

## Settings

Open Settings via `File > Preferences > Settings`.

### User Settings

When editing settings in the *User* tap all settings apply globally across all Visual Studio Code Workspaces.

### Workspace Settings

When editing settings in the *Workspace* tap all settings applied only effects the current opened workspace.

---

## Color Theme

You can customize the appearance of the Visual Studio Code interface to your needs. Navigate to the *Manage* tap in the Activity Bar and select `Color Theme`. There you can choose from a preinstalled Color Theme or install a new Color Theme with `+ Browse Additional Color Themes...`

---

## Debugging and testing

Visual Studio Code includes built-in support for debugging many languages, including JavaScript, TypeScript, and Python. To start debugging, you need to configure a "launch.json" file, which tells Visual Studio Code how to start and attach to your application. Once you have a launch configuration set up, you can start debugging by clicking the play button in the debug view or by pressing F5.

---

## Source Control

Visual Studio Code support source control systems like Git, SVN, and TFS. The source control icon will appear on the left sidebar once you open a folder that is a git repository, allowing you to see the changes, make commits and handle merge conflicts, among other functionalities.

---

These are just a few of the many features that Visual Studio Code has to offer. With its powerful editing capabilities, built-in support for debugging and testing, and integration with source control, Visual Studio Code is a great choice for a wide range of development tasks. As you become more familiar with the tool, you'll find that it can help you work more efficiently and effectively.

---

[Next Chapter](UsingVSCodeWithObjectScript.md)

[Overview](../README.md)

by [Philipp B.](https://github.com/phil1436)
