Path Translator
===============

Converts Windows style paths to Unix style paths and vice versa. Its a very simple feature, but think about the number of times you have had to do something like this and done it manually.

## What does it do?


####Windows to Unix
Takes a windows path, removes the drive letter a.k.a. C: and changes '\' to '/'.

####Unix to Windows
Find the unix prefix ('/cygdrive/' or '/'), take the following letter as a drive letter en adds this drive letter followed by ':' to  the path, changing '/' to '\'


## Installation

### By Package Control

1. Download & Install `Sublime Text 3` (https://www.sublimetext.com/3)
1. Go to the menu `Tools -> Install Package Control`, then,
   wait few seconds until the `Package Control` installation finishes
1. Go to the menu `Preferences -> Package Control`
1. Type `Package Control Add Channel` on the opened quick panel and press <kbd>Enter</kbd>
1. Then, input the following address and press <kbd>Enter</kbd>
   ```
   https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json
   ```
1. Now, go again to the menu `Preferences -> Package Control`
1. This time type `Package Control Install Package` on the opened quick panel and press <kbd>Enter</kbd>
1. Then, search for `PathTranslator` and press <kbd>Enter</kbd>

See also:
1. [ITE - Integrated Toolset Environment](https://github.com/evandrocoan/ITE)
1. [Package control docs](https://packagecontrol.io/docs/usage) for details.


## How do I use it?

####Usage
Highlight the path(s) to convert and select the appropriate command from the command palette. The two commands available are *"Path: Unix to Windows"* and *"Path: Windows to Unix"*.

You can also copy the path of the current file as Unix or Windows path to clipboard, using *"Path: Copy current file path as Unix"* or *"Path: Copy current file path as Windows"*

To configure the prefix of the Unix style path, edit the settings.
