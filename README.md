# R25-Python-Deprecated-Symbols-Finder

> :warning: This an archived legacy repository which is not actively maintained.

Provides a utility tool aimed at finding all Python symbols which have been deprecated in R25.

## Introduction

With Cinema 4D R25, around 1000 symbols were deprecated in Python. However rest assured, R25 is not going to be a hard break, and deprecated symbols will keep working for at least a year. Manually looking to a list of 1000 symbols within your files can be difficult, this is why we created this tool.

## Requirement

This plugin is released as it is and supports only R25. If you think there is an important missing feature or a bug please report to us at [developers.maxon.net](https://developers.maxon.net/). It is not in Maxon's priorities to maintains this tool.

## Installation

This is a regular CommandData plugin, install it within the Cinema 4D plugins folders.

## Usage

![R25 Python deprecated symbols finder](py_deprecated.jpg)

Go to the extension menu and click into the "R25 Python Deprecated Symbols Finder v1.0" menu entry.
Within the dialog go to the File menu and choose one of the options according to what you want to scan.
It will then scan folders, to search through *.c4d files, regular *.py files, and plugin files *.pyp.

The tool looks into the next elements of a Cinema 4D scene:

- Python Generator
- Python Effector
- Python Field Object
- Python Field Layer
- Python scripting Tag
- Python interaction tag
- Visual Selector tags are always reported since there is no API  to retrieve Python code.
- Python within an Xpresso tag (if the Python GvNode with the deprecated code live in a protected Xpresso Group, only the protected group is exposed)
- Character Component Tag
- Sketch Material using Python.
