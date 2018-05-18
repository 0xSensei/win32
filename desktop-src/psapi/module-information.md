---
title: Module Information
description: A module is an executable file or DLL.
ms.assetid: 'e15b5e15-ca06-4733-bd0a-705058ba2db8'
---

# Module Information

A *module* is an executable file or DLL. Each process consists of one or more modules. You can retrieve the list of module handles for a process by calling the [**EnumProcessModules**](enumprocessmodules.md) function. This function fills an array of **HMODULE** values with the module handles for the specified process. The first module is the executable file. Remember that these module handles are most likely from some other process, so you cannot use them with functions such as [**GetModuleFileName**](https://msdn.microsoft.com/library/windows/desktop/ms683197). However, you can use [PSAPI functions](psapi-functions.md) to obtain information about a module from another process.

The following procedure describes how to obtain module information from another process.

**To obtain module information from another process**

1.  Call the [**GetModuleBaseName**](getmodulebasename.md) function. This function takes a process handle and a module handle as input and fills in a buffer with the base name of a module (for example, Kernel32.dll). A related function, [**GetModuleFileNameEx**](getmodulefilenameex.md), takes the same parameters as input but returns the full path to the module (for example, C:\\Windows\\System32\\Kernel32.dll).
2.  Call the [**GetModuleInformation**](getmoduleinformation.md) function. This function takes a process handle and a module handle and fills a [**MODULEINFO**](moduleinfo-str.md) structure with the load address of the module, the size of the linear address space it occupies, and a pointer to its entry point.

If an application requires module information for the current process, it should use the [**GetModuleFileName**](https://msdn.microsoft.com/library/windows/desktop/ms683197) function instead of the PSAPI module functions. This helps application performance in two ways: The **GetModuleFileName** function is more efficient than the PSAPI module functions, and an application can avoid loading psapi.dll if it does not use any PSAPI functions.

The [**GetModuleBaseName**](getmodulebasename.md) and [**GetModuleFileNameEx**](getmodulefilenameex.md) functions are primarily designed for use by debuggers and similar applications that must extract module information from another process. If the module list in the target process is corrupted or is not yet initialized, or if the module list changes during the function call as a result of DLLs being loaded or unloaded, these functions may fail or return incorrect information.

 

 



