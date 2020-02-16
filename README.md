# MicVolumeLocker

Tired of those apps adjusting your microphone volume level without your permission ?
This script is for you, it acts like a daemon
which will loop and lock your volume level to a chosen one. (by default 100%)

## Getting Started

This script is for Windows and has been tested on Windows 10 only but it should work on earlier versions.

### Prerequisites

Requires [Nircmd](https://www.nirsoft.net/utils/nircmd.html).

### Installing

1. Download Nircmd and put ``nircmdc.exe`` into your ``PATH``, e.g. ``C:\Windows\``.

2. ``lock_micro_daemon.exe`` is the daemon, you only need this executable if you want to let the volume at 100%.

3. (Optional) ``lock_micro_src.bat`` is the source code used in the daemon (you don't need it, but if you want to change the microphone volume level (65535), you'll have to experiment your own values and compile that bat into an executable, also if you want to make it windowless you'll have to look for some software. I used [``Advanced Bat To Exe Converter``](http://www.battoexeconverter.com/)).

4. Put ``lock_micro_daemon.exe`` or the executable you might have created at step 3 in your startup folder.

### Notes

* Windows 10 Startup folder for current user

```text
C:\Users\<Username>\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup
```

* Windows 10 Startup folder for all users

```text
C:\ProgramData\Microsoft\Windows\Start Menu\Programs\StartUp
```