# 01 Installing the Domain Controller

1. Use `SConfig` to:
    - Change the hostname
    - Change the IP address to static
    - Change the DNS server to the IP of the domain controller


2. Install the Active Directory Windows Feature

```powershell
Install-WindowsFeature AD-Domain-Services -IncludeManagementTools
```


3. Configure Active Directory

```powershell
Import-Module -Name ADDSDeployment
Install-ADDSForest
```

