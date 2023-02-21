# Chocolatey Install

[https://chocolatey.org/install](https://chocolatey.org/install)

```sh

@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"

choco upgrade chocolatey

choco –version
choco --help
choco list --local-only
 * list - lists remote or local packages
 * search - searches remote or local packages (alias for list)
 * find - searches remote or local packages (alias for search)
 * info - retrieves package information. Shorthand for choco search pkgname --exact --verbose
 * install - installs packages from various sources
 * pin - suppress upgrades for a package
 * outdated - retrieves packages that are outdated. Similar to upgrade all --noop
 * upgrade - upgrades packages from various sources
 * uninstall - uninstalls a package
 * pack - packages up a nuspec to a compiled nupkg
 * push - pushes a compiled nupkg
 * new - generates files necessary for a chocolatey package from a template
 * sources - view and configure default sources (alias for source)
 * source - view and configure default sources
 * config - Retrieve and configure config file settings
 * features - view and configure choco features (alias for feature)
 * feature - view and configure choco features
 * setapikey - retrieves, saves or deletes an apikey for a particular source (alias for apikey)
 * apikey - retrieves, saves or deletes an apikey for a particular source
 * unpackself - have chocolatey set itself up



```

# Chocolatey package install

[https://chocolatey.org/packages](https://chocolatey.org/packages)

```sh

choco install tektoncd-cli --confirm

# choco install googlechrome --Yes --confirm --accept-license

choco install adobereader --Yes --confirm --accept-license  --verbose 

choco install firefox --Yes --confirm --accept-license
choco install adblockplus-firefox --Yes --accept-license
choco install notepadplusplus.install  --Yes --confirm --accept-license

choco install vlc --Yes --confirm --accept-license
choco install git.install --Yes --confirm --accept-license
choco install gh --Yes --confirm --accept-license
 
choco install curl --Yes --confirm --accept-license
choco install putty.install --Yes --accept-license
choco install winscp --Yes --confirm --accept-license
choco install openssh --Yes --confirm --accept-license
choco install openssl.light --Yes --accept-license
choco install keepass --Yes --accept-license

choco install golang --Yes --confirm --accept-license
choco install python3 --Yes --confirm --accept-license
choco install nodejs.install --Yes --confirm --accept-license
# choco install kotlinc install --Yes --accept-license
choco install php --Yes --accept-license

#Choose 1 Java package (Java 8 or Java 11 ) among the ones below :
#choco install adoptopenjdk8 --Yes --accept-license
#choco install openjdk --Yes --accept-license --version 11.0.2.01
#choco install zulu --Yes --accept-license --version 11.29.11
#choco install zulu11 --Yes --accept-license
choco install microsoft-openjdk11 --Yes --accept-license 
choco install microsoft-openjdk17 --Yes --accept-license 

choco install dotnetcore-sdk --Yes --confirm --accept-license
choco install dotnet --Yes --confirm --accept-license
choco install dotnet-sdk --Yes --confirm --accept-license
choco install nuget.commandline --Yes --accept-license
choco install vscode  --Yes --confirm --accept-license
choco install azure-cli --Yes --confirm --accept-license
choco install microsoftazurestorageexplorer --Yes --confirm --accept-license
choco install terraform --Yes --confirm --accept-license
choco install packer --Yes --confirm --accept-license
 
choco install mysql.workbench --Yes --confirm --accept-license
choco install mysql-cli --Yes --confirm --accept-license
choco install psql --Yes --confirm --accept-license
choco install mysql-connector --Yes --accept-license
choco install sqljdbc --Yes --accept-license
choco install sqlserver-odbcdriver --Yes --accept-license
choco install pgadmin3 --Yes --confirm --accept-license
choco install pgadmin4 --Yes --confirm --accept-license

choco install maven --Yes --confirm --accept-license
choco install gradle --Yes --confirm --accept-license
choco install postman  --Yes --confirm --accept-license
choco install selenium-all-drivers --Yes --accept-license
choco install ant --Yes --confirm --accept-license

choco install wireshark --Yes --confirm --accept-license
choco install sysinternals --Yes --confirm --accept-license

choco install kubernetes-cli --Yes --confirm --accept-license
choco install docker-desktop --Yes --confirm --accept-license
choco install minikube --Yes --confirm --accept-license
choco install kubernetes-helm --Yes --confirm --accept-license

choco install wsl-ubuntu-2004 --Yes --confirm --accept-license

choco install androidstudio --Yes --confirm --accept-license

choco install awstools.powershell --Yes --accept-license
choco install awscli --Yes --accept-license

```

# Chocolatey upgrade :

```sh

choco upgrade adobereader --Yes --confirm --accept-license
choco upgrade googlechrome --Yes --confirm --accept-license
choco upgrade firefox --Yes --confirm --accept-license
choco upgrade adblockplus-firefox --Yes --accept-license
choco upgrade notepadplusplus.install --Yes --confirm --accept-license
choco upgrade vlc --Yes --confirm --accept-license
choco upgrade git --Yes --confirm --accept-license
choco upgrade gh --Yes --confirm --accept-license
choco upgrade curl --Yes --confirm --accept-license
choco upgrade putty --Yes --accept-license
choco upgrade winscp --Yes --confirm --accept-license
choco upgrade openssh --Yes --confirm --accept-license
choco upgrade openssl.light --Yes --accept-license
choco upgrade keepass --Yes --accept-license
choco upgrade golang --Yes --confirm --accept-license
choco upgrade python3 --Yes --confirm --accept-license
choco upgrade nodejs --Yes --confirm --accept-license
choco upgrade php --Yes --accept-license

choco upgrade dotnetcore-sdk --Yes --confirm --accept-license
choco upgrade nuget.commandline --Yes --accept-license
choco upgrade vscode  --Yes --confirm --accept-license

choco upgrade azure-data-studio --Yes --confirm --accept-license
azdata cli 
choco upgrade azure-cli --Yes --confirm --accept-license

choco upgrade aks-engine --Yes --confirm --accept-license
choco upgrade microsoftazurestorageexplorer --Yes --confirm --accept-license
choco upgrade terraform --Yes --confirm --accept-license
choco upgrade packer --Yes --confirm --accept-license
choco upgrade wsl --Yes --confirm --accept-license
 
choco upgrade mysql.workbench --Yes --confirm --accept-license
choco upgrade mysql-connector --Yes --accept-license
choco upgrade sqljdbc --Yes --accept-license
choco upgrade sqlserver-odbcdriver --Yes --accept-license
choco upgrade pgadmin3 --Yes --confirm --accept-license
choco upgrade pgadmin4 --Yes --confirm --accept-license


choco upgrade maven --Yes --confirm --accept-license
choco upgrade gradle --Yes --confirm --accept-license
choco upgrade ant --Yes --confirm --accept-license
choco upgrade postman  --Yes --confirm --accept-license
choco upgrade selenium-all-drivers --Yes --accept-license


choco upgrade wireshark --Yes --confirm --accept-license
choco upgrade sysinternals --Yes --confirm --accept-license

choco upgrade kubernetes-cli --Yes --confirm --accept-license
choco upgrade docker-desktop --Yes --confirm --accept-license
choco upgrade minikube --Yes --confirm --accept-license
choco upgrade kubernetes-helm --Yes --confirm --accept-license

choco upgrade androidstudio --Yes --confirm --accept-license
choco upgrade awstools.powershell --Yes --accept-license
choco upgrade awscli --Yes --accept-license

```


# Enabling Hyper-V

https://blog.zwindler.fr/2018/10/02/minikube-sur-hyper-v-part-2-troubleshooting-de-linstallation/ 
https://minikube.sigs.k8s.io/docs/start/windows/
run CMD systeminfo
Open a PowerShell console as Administrator, and run the following command:


```sh
C:\Windows\SysWOW64\WindowsPowerShell\v1.0\powershell.exe -ExecutionPolicy Bypass -NoExit 
Get-ExecutionPolicy
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Hyper-V -All

New-VMSwitch -name MiniKubeExternalSwitch -NetAdapterName Ethernet -AllowManagementOS $true
Get-NetAdapter -Name * -Physical
New-VMSwitch -name DockerExternalSwitch -NetAdapterName Wi-Fi -AllowManagementOS $true

```

After some troubleshooting and head banging, it became apparent that the external network adapter had an ethernet adapter selected that was not connected to a network. (ethernet selected, instead of the wireless adapter). Of course an IP wont be allocated on an external network if none is connected.

```sh
minikube config set hyperv-virtual-switch MiniKubeExternalSwitch
minikube config set vm-driver hyperv
minikube config set memory 4096

minikube start --disk-size 10g --memory 4096 --alsologtostderr --v 9999

```

https://kubernetes.io/docs/setup/learning-environment/minikube/#using-minikube-with-an-http-proxy
https://kubernetes.io/docs/concepts/containers/images/#using-a-private-registry
https://minikube.sigs.k8s.io/docs/reference/persistent_volumes/
disk at C:\Users\$USERNAME\.minikube\machines\minikube\minikube\Virtual Machines

Install a local Docker registry:
https://docs.docker.com/registry/deploying/


```sh
wmic csproduct get identifyingnumber
wmic bios get serialnumber
wmic csproduct get name
```


