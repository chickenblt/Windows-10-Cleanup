<h1>Windows 10 de-bloat command</h1>

This powershell script will remove all windows 10 apps apart from edge and connect and the core windows 10 programs

If you delete too much stuff, create a new user and all the apps will come back

Command: 

Get-AppxPackage | Remove-AppxPackage
