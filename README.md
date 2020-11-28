# How to change the Windows default font

This guide asumes you want to replace the default Windows font with the font used by [Ubuntu](https://design.ubuntu.com/font/)

1. Download the Ubuntu font from [this location](https://assets.ubuntu.com/v1/0cef8205-ubuntu-font-family-0.83.zip)
2. Unzip the file.
3. In Windows, select all font files and right-click to install them.
4. Create a new registry file and put the following in it:
```
Windows Registry Editor Version 5.00

[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\Fonts]
"Segoe UI (TrueType)"=""
"Segoe UI Bold (TrueType)"=""
"Segoe UI Bold Italic (TrueType)"=""
"Segoe UI Italic (TrueType)"=""
"Segoe UI Light (TrueType)"=""
"Segoe UI Semibold (TrueType)"=""
"Segoe UI Symbol (TrueType)"=""

[HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows NT\CurrentVersion\FontSubstitutes]

"Segoe UI"="Ubuntu"
```
5. Save this file and merge it.
6. Reboot Windows. You're font should now be changed.
