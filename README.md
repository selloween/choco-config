# chocolatey.config
This is a chocolatey export of common packages install on my Windows machines.
You can adjust this config by removing package xml nodes accordingly.
Chocolatey is a awesome package manager for Windows that makes auto installing applications a breeze.
I've listed some basic examples on how to install and use chocolatey.
More info on how to install and use chocolatey here: https://chocolatey.org/ and https://github.com/chocolatey

### Install Chocolatey
Open Admin Powershell and paste:
```
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

### Adjust chocolatey.config
Remove package nodes you don't need.
```
<?xml version="1.0" encoding="utf-8"?>
<packages>
  <package id="7zip.install" version="18.5.0.20180730" />
  <package id="adobereader" version="2018.011.20063" />
  <package id="anaconda3" version="5.3.1" />
  <package id="azure-cli" version="2.0.52" />
  <package id="calibre" version="3.35.0" />
  <package id="ccleaner" version="5.50.6911" />
  <package id="chocolatey" version="0.10.11" />
  <package id="chocolatey-core.extension" version="1.3.3" />
  <package id="chocolatey-misc-helpers.extension" version="0.0.3" />
  <package id="chocolatey-windowsupdate.extension" version="1.0.3" />
  <package id="chocolateygui" version="0.16.0" />
  <package id="chromium" version="71.0.3578.80" />
  <package id="Cmder" version="1.3.10" />
  <package id="curl" version="7.62.0" />
  <package id="docker" version="18.09.0" />
  <package id="docker-compose" version="1.23.2" />
  <package id="docker-desktop" version="2.0.0.0" />
  <package id="DotNet4.5.2" version="4.5.2.20140902" />
  <package id="emacs" version="26.1.0.20180701" />
  <package id="Firefox" version="64.0" />
  <package id="git.install" version="2.20.0" />
  <package id="GoogleChrome" version="71.0.3578.80" />
  <package id="heidisql" version="9.5.0.5196" />
  <package id="javaruntime" version="8.0.191" />
  <package id="jre8" version="8.0.191.20181114" />
  <package id="KB2919355" version="1.0.20160915" />
  <package id="KB2919442" version="1.0.20160915" />
  <package id="KB2999226" version="1.0.20181019" />
  <package id="KB3033929" version="1.0.4" />
  <package id="KB3035131" version="1.0.2" />
  <package id="keepassxc" version="2.3.4" />
  <package id="MarkdownMonster" version="1.14" />
  <package id="minishift" version="1.28.0" />
  <package id="nodejs-lts" version="10.14.2" />
  <package id="nvm" version="1.1.5" />
  <package id="nvm.portable" version="1.1.7" />
  <package id="openshift-cli" version="3.11.0" />
  <package id="openssh" version="7.7.2.1" />
  <package id="owncloud-client" version="2.5.1.10973" />
  <package id="php" version="7.3.0" />
  <package id="python3" version="3.7.1" />
  <package id="rambox" version="0.6.3" />
  <package id="rufus" version="3.4" />
  <package id="steam" version="3.0.1.20181204" />
  <package id="teamviewer" version="14.0.13880" />
  <package id="vcredist140" version="14.16.27012.6" />
  <package id="vcredist2010" version="10.0.40219.2" />
  <package id="vim" version="8.0.604" />
  <package id="vlc" version="3.0.4" />
  <package id="vscode" version="1.29.1" />
  <package id="vscode-docker" version="1.0.0.20181011" />
  <package id="vscode-powershell" version="1.0.0.20181011" />
  <package id="Wget" version="1.20" />
  <package id="winscp.install" version="5.13.6" />
  <package id="wireshark" version="2.6.5" />
  <package id="yarn" version="1.12.3" />
</packages>
```

### Install packages from source file
Run in Admin Powershell or CMD to install applications:
```
choco install -y source chocolatey.config
```
### Update all packages
```
choco update
````

### Update specific packages
```
choco update firefox vscode emacs
```

### Add packages example
```
choco install -y firefox vscode emacs
```

### Remove packages example
```
choco uninstall -y firefox vscode emacs
``` 

