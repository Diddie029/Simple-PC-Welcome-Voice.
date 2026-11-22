# A simple PC Welcome Voice

A simple Windows startup voice assistant built with **PowerShell**. It automatically welcomes the user with a spoken message whenever they log into their PC.

## Features
- Automatically runs when Windows starts (at user login).
- Plays a custom welcome message.
- Uses Windows built-in Text-to-Speech (TTS).
- No additional software or installations required.

## Requirements
- Windows 10 or Windows 11.
- PowerShell.
- Windows Task Scheduler.

## Setup

1. Create a PowerShell file named `welcome.ps1`.
2. Add your custom welcome message.
3. Open Windows Task Scheduler (`taskschd.msc`).
4. Create a new task triggered **At log on**.
5. Set `powershell.exe` as the program.
6. Add the script path as an argument:

```powershell
-WindowStyle Hidden -ExecutionPolicy Bypass -File "C:\Path\To\welcome.ps1"
```

7. Save the task and restart or log out and back in.

## Customization

Edit the message inside `welcome.ps1` to change what your PC says when you log in.

## Technologies Used
- PowerShell
- .NET System.Speech
- Windows Task Scheduler

---

*A small project that makes every Windows startup feel a little more personal.*
