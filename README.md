# The basics

## Config Changes

### High Performance Power Plan

```
$powerPlan = Get-WmiObject -Namespace root\cimv2\power -Class Win32_PowerPlan -Filter "ElementName = 'High Performance'"; $powerPlan.Activate(); tzutil /s 'Central Standard Time'
```
### Central Time Zone

```
tzutil /s 'Central Standard Time'
```

## Choco installs

### Choco
```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
```
### Baseline Programs (I want this on every Computer)

```
choco install 7zip notepadplusplus -y
```

### Web Browsers

```
choco install googlechrome firefox /RemoveDistrubtionDir  microsoft-edge -y

```
choco install adobereader -y
choco install dropbox -y
```

```
choco install office365homepremium -y
```

