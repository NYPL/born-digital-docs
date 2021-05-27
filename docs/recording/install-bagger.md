---
layout: default
title: Install Bagger
nav_order: 2
parent: Recording
---

## Introduction
Bagger is a graphical user interface that can package files using the Library of Congress BagIt File Packaging Format. Use Bagger when you prefer not to use a command line interface.

This document includes instructions for Windows and Mac.  

Bagger requires Java. Instructions for Java are included in this document.
## Using Bagger
Create a submission package after any applicable service copies have been [reviewed]() and approved. Once folders are organized according to the [packaging standard](file-and-packaging-specifications.html) use Bagger to create a submission package.  

## Java
Before installing Bagger check the computer's Java Runtime Environment.
### Windows
#### Confirm Java is installed
* Navigate to Control Panel.
* Double-click on Java to open the Java Control Panel.
* Select the Java tab and then select the View button.  
* Check that a Java Product and Path are displayed.  

#### Confirm JAVA_HOME variable is set
* Navigate to Control Panel.
* Select System and then select the Advanced tab. 
* Select the Environment Variables button.  
* Scroll through System variables to find JAVA_HOME.

#### Create JAVA_HOME variable if not defined and Java is installed
* Select the New button below System variables.
* Type JAVA_HOME in the Variable name field.
* Type the path to the Java folder in the Variable value field.
    * The Java folder has a name like jre followed by a number. This is the folder above the bin and lib folders in the Java package.
* Select OK to save and close.
* Scroll through System variables to find JAVA_HOME.

#### Install Java
* Navigate to Java [download](https://java.com/en/download/manual.jsp) page from a web browser.
* Select a Windows software download.  
* Select Save. Save to an easy to find location.
* Find and select the saved file.
* Select Install.
* Uncheck options to install additional software programs.
* Select Next.
* Select Close when the process is complete.
* Complete the steps from [Confirm Java is installed](install-bagger.html#confirm-java-is-installed) through Create JAVA_HOME as needed.  

#### Install Bagger
* Download the Latest release from [Library of Congress](https://github.com/LibraryOfCongress/bagger/releases/latest).
* Unzip the package to a location where you store programs on your computer.  
* Note the location. Create a shortcut to `\bagger-2.x\bin\bagger.bat`, alternatively.

#### Run Bagger
* Navigate to the location where Bagger is unzipped. `\bagger-2.x\bin\bagger.bat`.  
* Double-click bagger.bat  
OR 
* Double-click bagger shortcut.
* See [How to bag]() to create packages.

### Mac
#### Confirm Java is installed
* Navigate to System Preferences.
* Select Java. Java Control Panel will open in a new window.  
* Select the Java tab. Select the View button.  
* Check that a Java Product and Path are displayed.  

#### Install Java
* Navigate to Java [download](https://java.com/en/download/manual.jsp) page from a web browser.  
* Select a Mac software download.  
* Select Save. Save to an easy to find location.
* Find and select the saved file.
* Select Install.
* Uncheck options to install additional software programs.
* Select Next.
* Select Close when the process is complete.
* Complete the steps from [Confirm Java is installed](install-bagger.html#confirm-java-is-installed).

#### Install Bagger
* Download the Latest release from [Library of Congress](https://github.com/LibraryOfCongress/bagger/releases/latest).
* Unzip the package to Applications.  
* Create an alias to `\bagger-2.x\bin\bagger` and move it to a convenient location, if preferred.

#### Run Bagger
* Navigate to the location where Bagger is unzipped. `\bagger-2.x\bin\bagger.`.  
* Double-click bagger.  
OR 
* Double-click bagger alias.
* See [How to bag]({% link docs/recording/how-to-bag.md %}) to create packages.