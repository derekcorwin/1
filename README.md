powercfg -duplicatescheme 8c5e7fda-e8bf-4a96-9a85-a6e23a8c635c

tzutil /s 'Central Standard Time'

Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))

choco install 7zip notepadplusplus googlechrome -y

choco install adobereader -y
choco install dropbox -y

choco install office365homepremium -y


