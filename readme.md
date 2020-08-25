<h1>Windows 10 de-bloat command</h1>

This powershell script will remove all windows 10 apps apart from edge and connect and the core windows 10 programs

The store will stay! You can add specific programs such as xbox or photos after you run this by going to the store and downloading them!


Command: 

Get-AppxPackage -AllUsers | where-object {$_.name -notlike "*Microsoft.WindowsStore*"} | where-object {$_.name -notlike "*Microsoft.WindowsCalculator*"} | Remove-AppxPackage
