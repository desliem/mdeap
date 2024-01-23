# MDeap 2

**Version 2.0.0.1**  
**© copyright 2015 Michel Deslierres**

**MDeap 2** is a convivial self contained Windows application capable of calculating basic data envelopment models (DEA). It can calculate CCR and BCC models with input or output orientation. In the case of BCC models, returns to scale can be constant, non increasing, non decreasing, variable or general (bounded). It can also calculate allocative efficiency (cost and revenue). The linear programs are solved with the **lp_solve** library version 5.5 (included in the installation). 

**MDeap 2** is a 32-bit Windows application. It has been tested on Windows and 8.1 (64 bit) but it probably runs on all versions of Windows starting with Windows XP.

**Content**

<!-- TOC -->

- [1. Installation](#1-installation)
  - [1.1. Types of installation](#11-types-of-installation)
  - [1.2. Instructions](#12-instructions)
- [2. Example files](#2-example-files)
- [3. Instructions for use of **MDeap 2**](#3-instructions-for-use-of-mdeap 2)
- [4. DISCLAIMER and WARNING](#4-disclaimer-and-warning)
- [5. Removing **MDeap 2**](#5-removing-mdeap 2)
- [6. Acknowledgement](#6-acknowledgement)
- [7. Latest changes](#7-latest-changes)

<!-- /TOC -->

## 1. Installation

The installation program for the latest version of **MDeap 2** is available here: [MDeap2Install-2-0-0-1.exe](bin/MDeap2Install-2-0-0-1.exe). Click on the link.

![](../img/download_installer.png)

Then click on the `Download raw file` icon as shown above. Once the executable is downloaded, verify its checksum. 

| Hash   | MDeap2Install-2-0-0-1.exe checksum  |
|---   |--- |
| md5  | 7d1fc8f52ce51ae18cbec0c49084a5c3 |
| sha1 | 9408bb1c994d6d95d0acb8fb3fd693ee9e776e80 |


### 1.1. Types of installation

**MDeap 2** can be run as a "standard" Windows' application or as a "portable" application. 

  - A standard application of **MDeap 2** will associate `.wdjson` files to itself which requires modifying Windows' registry. Furthermore, the standard folders will be used to store the application's configuration file and the application's data files.

  - A portable application of **MDeap 2** will make no changes to Windows' registry. By default, the application's configuration file and data files will be stored in the folder containing the application.  

    Most often, a portable program is installed on removable media such as thumb drives. But it is entirely possible to choose to perform a portable installation in a hard drive's folder. Just make sure that you have full read and write rights on that folder. 

The type of installation is specified at the very end of the installation process.

### 1.2. Instructions
 
  1.  Select the installation language (English or French). This is the language used by the installation program and has nothing to do with the language used in **MDeap 2**.

  1.  Read the Welcome screen and click on `Next >`.

  1.  Read the License Agreement, select `I accept the agreement` if you do and then click on `Next >`.

  1.  Select the destination folder.
       -  For a standard installation, you can probably accept the default location.
       -  For a portable installation, browse to a folder where you have full read and write permission. That excludes folders `Windows`, `Program Files` and, on 64 bit systems, `Program files (x86)`. 

  1. Select the start menu folder.
       -  For a standard installation, you can probably accept the default location.
       -  For a portable installation, accept the default, it will be ignored in any case as nothing will be added to the start menu.

  1. Select the type of installation (standard or portable). It is also possible to include national language support or not. Currently **MDeap 2** is available in two languages: English and French. It will be possible to translate to other languages if national language support is included.

  1. Finally, click on the `Install` button and, once the installation is completed, click on the `Finish` button.

If a standard installation was chosen, the extension `.wdjson` will be associated with **MDeap 2** which will cause `Win4Dep2.exe` to be launched whenever a file with that extension is double clicked. Also an uninstall program will be installed. Finally, a menu item will be added to the Start menu. If a portable installation was selected, the file association will not be performed, a menu item and the uninstall program will not be created.


## 2. Example files

Some example project files are provided in **MDeap 2** format (extension `.mdjson`). They are in a folder called, appropriately, `Examples`. In a standard installation, that folder will be `MDeap2` a folder contained in the `Documents` folder. In a portable installation, `Examples` will be in the folder containing `MDeap2.exe`.


## 3. Instructions for use of **MDeap 2**

**MDeap 2**'s help file is not complete. Nevertheless it should not be too difficult to figure out how it works.

The application provides a grid not unlike a spreadsheet to enter and edit data. Multiple DEA models can then be applied against the data set or subsets of it. Specification of models is a point and click operation. Results are shown in a series of tables that can easily be copied to other applications.

Press F1 to get contextual help, when available.

 **MDeap 2** can read **Win4Deap 2** project files and vice versa.

## 4. DISCLAIMER and WARNING

**MDeap 2** is free software that is provided as is. The author of the program accepts no responsibility for any damages that could be caused by this software and makes no warranty, whether implied or implicit, about its fitness for any purpose. The user assumes all risks associated with the program. Please read the copyright notice and license agreement for more.

**MDeap 2** should be considered beta software. Backup data often and in both the native `wdjson` format and standard CSV formats.


## 5. Removing **MDeap 2**

An uninstall program is installed along with `MDeap2.exe` if a standard installation was performed. If a portable installation was chosen, manually delete the installed files. No changes were made to the system in that case.

## 6. Acknowledgement

All the linear programming models needed for DEA calculations are done by the  **lp_solve** library.(released under the LGPL 2.1 license). It can be found can be found at https://lpsolve.sourceforge.net/.

Thanks to Jordan Russell for the Inno Setup Compiler which was used to create the installation program. The setup compiler can be found on the Web at http://www.innosetup.com. 

Most of the icons are from the Silk icon set by Mark James released under the Creative Commons Attribution 2.5 License: ~~http://www.famfamfam.com/lab/icons/silk/~~ no longer online, but see https://github.com/legacy-icons/famfamfam-silk.

The application's icon was created with the open source application Greenfish Icon Editor Pro:  http://greenfishsoftware.org/.


## 7. Latest changes

Version 2.0.0.1 Changed version number to 2 to concord with the application's name and fixed many minor bugs.

Version 0.9.3.2 Many bug fixes including error while importing csv files with prices, errors with filenames with non ascii characters. Completed HTML export of all tables and added saving all model tables to csv files.

Version 0.9.2.11 - first released version
