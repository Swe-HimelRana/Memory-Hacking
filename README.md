# Installing tools

We will use a Boxstarter script to install some game hacking tools. Boxstarter is a set of utilities that allows you to script and recreate installations. In this case, we will use it to install a memory searcher and debugger. Within your VM, open up Powershell and run the following two commands:

```powershell
. { iwr -useb https://boxstarter.org/bootstrapper.ps1 } | iex; Get-Boxstarter -Force
```

```powershell
Install-BoxstarterPackage -PackageName https://raw.githubusercontent.com/Swe-HimelRana/Memory-Hacking/main/vmsetup.txt -DisableReboots
```

The first command installs BoxStarter and is taken from their website. The second command is a setup script that enables some folder options and installs three programs:

1.  Cheat Engine, a memory scanner
2.  x64dbg, a debugger
3.  Chocolatey, a package manager

As you discover more tools, you should create your own script and add them.
