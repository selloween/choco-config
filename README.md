# chocolatey.config
This is a chocolatey export of common packages install on my Windows machines.
You can find more info on how to install and use Chocolatey here: https://chocolatey.org/

### Install Chocolatey
Open Admin Powershell and paste:
```
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

### Install packages
Run in Admin Powershell or CMD to install applications:
```
choco install -y source chocolatey.config
````

### Update packages
```
choco update
````
