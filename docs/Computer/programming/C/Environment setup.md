# Environment setup
## Tools
- MinGW
- PowerShell
- Windows Terminal

## Steps
1. Download and install [MinGW](https://mingw.osdn.io) or a custom version [here](https://nuwen.net/mingw.html)
2. Set envi parameters for MinGW using powershell

```PS
$INCLUDE = "C:\MinGW\bin"

$OLDPATH = [System.Environment]::GetEnvironmentVariable('PATH','machine')
$NEWPATH = "$OLDPATH;$INCLUDE"
[Environment]::SetEnvironmentVariable("PATH", "$NEWPATH", "Machine")

```

You can now use MAKE and GCC.