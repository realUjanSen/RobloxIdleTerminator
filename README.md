```
  ____       _     _             ___    _ _        _____                   _             _             
 |  _ \ ___ | |__ | | _____  __ |_ _|__| | | ___  |_   _|__ _ __ _ __ ___ (_)_ __   __ _| |_ ___  _ __ 
 | |_) / _ \| '_ \| |/ _ \ \/ /  | |/ _` | |/ _ \   | |/ _ \ '__| '_ ` _ \| | '_ \ / _` | __/ _ \| '__|
 |  _ < (_) | |_) | | (_) >  <   | | (_| | |  __/   | |  __/ |  | | | | | | | | | | (_| | || (_) | |   
 |_| \_\___/|_.__/|_|\___/_/\_\ |___\__,_|_|\___|   |_|\___|_|  |_| |_| |_|_|_| |_|\__,_|\__\___/|_|   
                                                                                                       
```
                                                                                                                                                                   
                                                                                                        
Version: 1.0.0

Released: May 19, 2025

Author: Ujan Sen

GitHub: https://github.com/realUjanSen/RobloxIdleTerminator




 What is this tool?

A lightweight Windows executable that calculates when Roblox has disconnected you from a game server 
due to 20 minutes of inactivity, and then automatically closes the Roblox client if it stays 
disconnected for at least 30 seconds.


 Why did I make this?

Roblox leaves the client running and using resources after disconnecting for inactivity, 
Most Roblox users don’t have Python installed and shouldn’t need to. 
No official or community solution existed-so I built this to fill that gap.


 Why you might need this tool:

Many Roblox players go AFK (away from keyboard) mid-game and never return. While Roblox will 
disconnect you from the server after about 20 minutes of inactivity, the Roblox client continues 
running all local game logic, animations, and scripts-consuming significant CPU, GPU, and 
memory resources. This is very different from simply browsing Roblox, which uses minimal 
system resources.

If you leave Roblox running in this disconnected state for hours (for example, overnight), your 
computer-especially laptops-can experience sustained high CPU and GPU temperatures. This can lead 
to hardware damage, reduced performance, system instability, battery stress, and, in extreme cases, 
even fire risk-particularly if a laptop is left on a soft surface without proper ventilation.

RobloxIdleTerminator is a standalone executable that automatically closes Roblox after it’s 
been idle and disconnected, freeing up your system resources and protecting your hardware from 
the risks of prolonged overheating and resource hogging.  



⚠️ Big Scary Windows Warning (Thanks, Microsoft)

When you try to run this program, Windows will probably freak out and throw a giant red box at you 
saying “Unknown Publisher” or “This software might harm your computer.” Why? Because Microsoft 
wants me to cough up hundreds of dollars a year for a code signing certificate-just to make that 
warning disappear-even for free, open-source projects like this.

I’m not a company. I’m not selling anything. I’m not about to pay Microsoft (and their certificate 
authority buddies) a yearly fee so they can “protect” you with a meaningless pop-up. Even if I did 
pay, Microsoft would still keep showing warnings until I “built up enough reputation,” whatever 
that means.

  How to bypass antivirus and run this tool:

1. Download the project as a ZIP file from GitHub to avoid your browser falsely flagging the EXE as 
a virus or blocking the download.

2. Extract the ZIP to a folder on your computer. AV's wont delete it yet.

3. When you run the EXE, click “Run anyway” if Windows shows a big red warning box. This is normal 
for unsigned programs.

If you don’t trust pre-built executables, you can always check the source code or build the EXE 
yourself using PyInstaller. Don’t let Microsoft’s security theater stop you from using a genuinely 
useful tool.

TL;DR:
Microsoft wants your money, not your safety. 
This tool is safe, open-source, and free-just not “signed.”

www.virustotal.com/gui/file/ebd5b21e64670a3672b00de07f7b5a75e9823b7666ec16b91028c5abe099d954

For security-conscious users:
If you don’t trust the prebuilt executable(as you should anyway), you can build it yourself. 
The source code and icon are included in the folder you can download from GitHub.

How to build your own executable:

1. Download the entire folder from GitHub. It will contain:

   RobloxTerminatorTool
   ├── RobloxIdleTerminator.py
   └── rb.ico

2. Open RobloxTerminatorTool folder in File Explorer.

3. Click on the address bar at the top, select all and type:

   > cmd
   and press Enter. This will open Command Prompt in that folder.

4. Run this command:

   > pyinstaller --noconsole --onefile --icon=rb.ico RobloxIdleTerminator.py

5. After the build is complete, open the 'dist' folder created inside the same directory. 
   You will see:

	RobloxIdleTerminatorTool
	│   rb.ico
	│   RobloxIdleTerminator.py
	│   RobloxIdleTerminator.spec
	│
	├───build
	│   └───RobloxIdleTerminator
	│       │   Analysis-00.toc
	│       │   base_library.zip
	│       │   EXE-00.toc
	│       │   PKG-00.toc
	│       │   PYZ-00.pyz
	│       │   PYZ-00.toc
	│       │   RobloxIdleTerminator.pkg
	│       │   warn-RobloxIdleTerminator.txt
	│       │   xref-RobloxIdleTerminator.html
	│       │
	│       └───localpycs
	│               pyimod01_archive.pyc
	│               pyimod02_importers.pyc
	│               pyimod03_ctypes.pyc
	│               pyimod04_pywin32.pyc
	│               struct.pyc
	│
	└───dist
	        RobloxIdleTerminator.exe


Open this file in the following directory:
   dist
   └── RobloxIdleTerminator.exe

6. Double-click the .exe file to run it.narendra pur college indraneel, ac , travarsa


 For Mac and Linux users:

While the EXE is for Windows, you can run the Python script directly on other operating 
systems (as long as you have Python installed). Some features may be Windows-specific.
