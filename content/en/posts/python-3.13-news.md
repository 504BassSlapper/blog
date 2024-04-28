---
author: KittyCatPixel
title: Python 3.13 news
date: 2024-06-17T12:00:06+09:00
description: tabs, code-tabs, expand, alert, warning, notice, img, box
draft: false
hideToc: false
enableToc: true
enableTocContent: true
tocPosition: inner
authorEmoji: 👽
image: images/feature3/code-file.png
libraries:
- katex
---

## Python 3.13: What is upcomming 

Python 3.13.0a0 is currently in development and includes a number of new features and improvements. In this blog post, we’ll look at some of the new Python 3.13.0a0 features and provide some sample code to get you started.

The most recent version is 3.11.4, and 3.12 is in early preview. You can better understand Python 3.13.0a0 by reading these articles about Python 3.11.4 and Python 3.12.

New Features
There are no new modules yet, but there are some improved modules; they are array, io, pathlib, traceback, typing.

array: 'w' type code is available to be used for Unicode strings.
io: close() method of theio.IOBase finalizer now logs errors with sys.unraisablehook.
pathlib: Added changes to pathlib.PurePath.match(), pathlib.Path.glob() and rglob().
tracebackThe show_group parameter was added to traceback.TracebackException.format_exception_only().
typing: typing.get_protocol_members() was added to the set of members defining a typing.Protocol. typing.is_protocol() was added to check whether a class is a typing.Protocol.
Performance Optimizations
From PEP 594:

Deprecated Features
Deprecation of wave.Wave_read and wave.Wave_write methods
Deprecation of keyword arguments in creating typing.NamedTuple classes
Deprecation of functional syntax usage in creating typing.NamedTuple and typing.TypedDict classes
Deprecation of the array’s'u' format code.
Deprecation of ctypes.SetPointerType() and ctypes.ARRAY() functions
Removed Features
Removal of telnetlib module.
Removal of 2to3 program and lib2to3 module.
Removal of namespaces typing.io and typing.re.
Removal of webbrowser MacOSX class
Removal of support for using pathlib.Path object as context managers
Removal of configparser.LegacyINterpolation class.
Removal of turtle.RowTurtle.settiltangle() method.
Removal of certain unittest functions
Removal of cgi and cgitb modules
Removal of various modules and packages like sndhdr, pipes, ossaudiodev, mailcap, spwd, nntplib, nis, xdrlib, msilib, crypt, uu, aifc, audioop, chunk, imghdr, unittest.TestProgram.usageExit(), tkinter.tix, trashcan macros, locale.resetlocale(), logging.Logger.warn(), urllib.request.urlopen() parameters, webbrowser.MacOSXOSAScript._name attribute, re.template function, and re.TEMPLATE flag
C API Changes
Deprecated:
Deprecated old Python initialization functions such as

PySys_ResetWarnOptions()
PY_NAME_GetExecPrefix()
Py_GetPath()
Py_GetPrefix()
Py_GetProgramFullPath()
Py_GetProgramName()
Py_GetPythonHome()
Deprecated the Py_ImportModuleNoBlock() function, scheduled for removal in Python 3.15. Removed:
Removed
Removed functions deprecated in Python 3.9, such as PyEval_CallObject(), PyEval_CallObjectWithKeywords(), PyEval_CallFunction(), PyEval_CallMethod(), andPyEval_CFunction_Call().

The following old functions to configure the Python initialization, deprecated in Python 3.11, have been removed:

PySys_AddWarnOptionUnicode(): Use PyConfig.warnoptions instead.
PySys_AddWarnOption(): Use PyConfig.warnoptions instead.
PySys_AddXOption(): Use PyConfig.xoptions instead.
PySys_HasWarnOptions(): Use PyConfig.xoptions instead.
PySys_SetArgvEx(): Set PyConfig.argv instead.
PySys_SetArgv(): Set PyConfig.argv instead.
PySys_SetPath(): Set PyConfig.module_search_paths instead.
Py_SetPath(): Set PyConfig.module_search_paths instead.
Py_SetProgramName(): Set PyConfig.program_name instead.
Py_SetPythonHome(): Set PyConfig.home instead.
Py_SetStandardStreamEncoding(): Set PyConfig.stdio_encoding instead.
_Py_SetProgramFullPath(): Set PyConfig.executable instead.

