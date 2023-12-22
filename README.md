# ВОЗВРАТ

1. Открываем PowerShell, который в папке от имени администратора.
2. Копируем скрипт ниже, вставляем в PowerShell и запускаем.

Get-AppXPackage -allusers | Foreach {Add-AppxPackage -DisableDevelopmentMode -Register "$($_.InstallLocation)\AppXManifest.xml"}
