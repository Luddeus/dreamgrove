### How to build SimC command line interface on Windows 10

1. Install Visual Studio 2019 Community Edition from https://visualstudio.microsoft.com/downloads/ Download and run the installer. In the Workloads tab, select "Desktop development with C++". The optional features you must have are:
    * MSVC v142 - VS2019 C++ x64/x86 build tools
    * Windows 10 SDK (latest version)
2. Install git for Windows from https://git-scm.com/downloads Download and run the installer with default settings.
3. Open command prompt and goto the directory where you want to download the SimC source code.
4. Type in: git clone https://github.com/simulationcraft/simc.git
5. Type in: git checkout -b shadowlands
6. You will have a directory in the current directory called 'simc' with all the files.
7. Run Visual Studio 2019. Click "Open a project or solution" and select 'simc_vs2019.sln' in your 'simc' folder.
8. In the menu, select Build->Configuration Manager.
9. Select "Release-NoNetworking" as the active solution configuration from the downdown.
10. In the menu, select Build->Build Solution.
11. Once build is finished, goto your 'simc' folder. The simc command line executable is in '\simc\x64\Release-NoNetworking\simc_vs2019.exe'. Copy this to your 'simc' folder as "simc.exe".
12. To run SimC, from the command prompt type in: simc <profile file name>