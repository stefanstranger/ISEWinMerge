# Powershell ISE WinMerge ISE Add-On Module
- - -
This ISE Add-On adds integration with the WINMerge application into the ISE.

For more information about WinMerge go to: http://winmerge.org/

02/18/2015: - Initial version

![ScreenShot](https://raw.githubusercontent.com/stefanstranger/ISEWinMerge/master/isewinmergemodule.gif)

# Install

 1. Install WinMerge using PowerShell OneGet or manually from http://winmerge.org
 
 Default installation folder which module is looking for is 'C:\Program Files (x86)\WinMerge\WinMergeU.exe'
   If WinMerge is not installed in default folder change the following variable in ISEWinMerge.psm1 file.
   \# Configure location of WinMerge
   $global:exe = "C:\Program Files (x86)\WinMerge\WinMergeU.exe"
 2. Install ShowUI module from https://showui.codeplex.com/ or using PowerShell OneGet.
   OneGet installation:
   Find-Module ShowUi | Install-Module -verbose
 3. To install the module including all source code you can just run in a PowerShell v3 or higher the following command:
<pre>
iex (New-Object Net.WebClient).DownloadString("http://bit.ly/17h35mY")
</pre>

# Run
Run in PowerShell ISE

    Import-Module ISEWinMerge
    Start-ISEWinMerge

or hit Alt-W in ISE
