---
title: Accessing Your Project Workspace
description: Learn how to access and navigate your ADRF project workspace, including the virtual desktop environment and available software
order: 3
lastUpdated: 2025-03-31
---

# Accessing Your Project Workspace

A **project workspace** is a secure, isolated virtual environment in the ADRF within which an approved set of users can access a defined number of agency datasets. The project workspace is designed to allow approved researchers to access, analyze, and manipulate specific datasets relevant to their approved projects while maintaining strict data confidentiality and integrity.

Project workspaces in the ADRF are isolated from each other. Even if a person is granted access to two project workspaces, the user cannot access or copy files from one into the other. This is important because the two project workspaces might have access to different datasets.

## Virtual Desktop Environment

### What is a VDE?

A **virtual desktop environment (VDE)** allows you to interact with a remote system as if it were your own personal computer. The majority of your standard desktop functions are available, but the programs, data, and permissions are all controlled by the remote administrator (Coleridge Initiative). The ADRF uses a standard Windows environment (Windows Server) and provides a variety of software packages to conduct your analysis.

<!-- 
![Virtual Desktop Environment](/images/docs/use1.png)
-->

### Temporary Nature of the Environment

The environment is temporary in nature. This means that if you are not using it for a prolonged period of time (default is four hours but can vary by project), running programs will stop running and the information stored in temporary locations will be deleted. You will receive an on-screen message before any sessions are terminated.

**Important**: It is crucial to make sure that your work is saved—and saved in an appropriate location. Once this is complete and you are finished working, make sure that you log out of the ADRF instead of closing the window.

### The U: Drive and the P: Drive

**U: Drive (User Drive)**
- Your personal workspace that only you can access in the ADRF
- Folder name will include your Firstname and Lastname
- Store files you are working on individually
- 150GB storage limit

**P: Drive (Project Drive)**
- Used to house project-specific folders
- Accessible by all collaborators on the same project
- Use this drive to share files with team members
- 150GB storage limit

**Note**: The ADRF will not alert users when they approach the 150GB limit. Users can check their current usage by right-clicking on the user folder and clicking on properties.

### Toolbar and Settings

The top taskbar contains shortcuts to the command prompt, multiple desktop windows, a temporary folder, settings, full-screen view, and toggling multiple monitors.

<!--
![Taskbar](/images/docs/use2.png)
-->

### Windows Settings

Your desktop will look familiar if you are a Windows user. You will have icons for quick access to programs or browsers on your desktop. The windows icon on the bottom left side of the screen will open up a menu of programs, folders, and other tools. You will have access to PowerShell and several customization settings.

<!--
![Desktop](/images/docs/use3.png)
--> 

## Software in the ADRF

### JupyterLab

**JupyterLab** provides flexible building blocks for interactive, exploratory computing. While JupyterLab has many features found in traditional integrated development environments (IDEs), it remains focused on interactive, exploratory computing.

The JupyterLab interface on the ADRF consists of a main work area containing tabs of documents and activities, a collapsible left sidebar, and a menu bar. The left sidebar contains a file browser, the list of running terminals and kernels, the table of contents, and the extension manager.
<!--
![JupyterLab](/images/docs/use4.png)
-->
When using Jupyter Notebooks, make sure that all your work is saved to your U: drive and the correct directory within the U: drive. You can find the active directory by reading the path displayed in the file browser. By default, JupyterLab opens with your U: drive as the base directory.
<!--
![Make sure your work is saved to your U: drive](/images/docs/use5.png)
-->

#### Jupyter Notebooks

Jupyter Notebooks are documents that combine live runnable code with narrative text (Markdown), equations (LaTeX), images, interactive visualizations, and other rich output. You can create a notebook by clicking the blue + button in the file browser and then selecting a kernel (R, Python3, Stata) in the Launcher tab.

### Python 3

Python is a general-purpose programming language. You can access Python in multiple ways:

1. **Through JupyterLab** (Recommended) - Has packages installed and available, and an execution environment for testing and running code

<!--
![JupyterLab Python](/images/docs/use8.png)
-->

2. **Through the start menu** - Type in Python to access Python 3.7 (64-bit)

<!--
![Start menu](/images/docs/use6.png)
-->

3. **Through the command prompt** - Open command prompt from the top taskbar and type `python`

<!--
![Command Prompt](/images/docs/use7.png)
-->

4. **Through PyCharm**

<!--
![PyCharm](/images/docs/use9.png)
-->

### R

**R** is a general-purpose programming language. You may access R in one of three ways:

1. **Through RStudio** - An integrated development environment (IDE) for R. Open RStudio through the desktop shortcut.
2. **Through JupyterLab** - Click the R icon in your Launcher window
3. **Through the R GUI** - Type R in the search bar and click to open the RGui

### Stata

**Stata** is a general-purpose statistical software package. Stata can be accessed through the desktop shortcut StataMP 16 or by searching for it using the search or menu bar, or through JupyterLab.

### DBeaver

**DBeaver** is a universal tool for querying, editing, and managing data stored in Redshift databases. The ADRF stores data using AWS Redshift Server. DBeaver can be accessed through the desktop shortcut or by searching for it using the search bar.

Once open, you will need to connect to a Redshift server. Please contact ADRF support for connection details.


<br>

---
# Support & Navigation

**Need help?**
- Email: support@coleridgeinitiative.org
- Hours: Monday-Friday, 9 AM - 5 PM ET

**Navigation**
- ⬅️ [Back to Home](../README.md)

