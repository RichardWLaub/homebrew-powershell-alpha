# Powershell Alpha

Cask for installing alpha powershell on MacOS.

Install with:

```
brew cask install RichardWLaub/powershell-alpha/powershell-alpha
```

## Installing Azure Powershell

Launch powershell:

```bash
powershell
```

Install, import, and login with:

```powershell
Install-Package -Name AzureRM.NetCore.Preview -Source https://www.powershellgallery.com/api/v2 -ProviderName NuGet -ExcludeVersion -Destination /usr/local/share/powershell/Modules
Import-Module AzureRM.NetCore.Preview
Login-AzureRMAccount
```

Sources:

* https://blogs.technet.microsoft.com/jessicadeen/azure/getting-started-with-powershell-core-and-azurerm-modules-on-ubuntu-and-os-x/
* https://github.com/caskroom/homebrew-cask/blob/685ba1c3c89f2ee4058af9d40d0add1a46fb79f9/Casks/powershell.rb
