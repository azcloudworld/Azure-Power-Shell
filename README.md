# Azure-Power-Shell

Azure PowerShell Commands

Az PowerShell module is the recommended PowerShell module for managing Azure resources on all platforms.

Az PowerShell module is based on the .NET Standard, and works with PowerShell 7.0.6 LTS and PowerShell 7.1.3 or higher on all platforms including Windows, macOS, and Linux. It's also compatible with Windows PowerShell 5.1.

Install Azure PowerShell:

Install-Module -Name Az -Scope CurrentUser -Repository PSGallery -Force

Install PowerShell Get :

Install-Module -Name PowerShellGet
Install a module only for the current user
Install-Module -Name PowerShellGet -Scope CurrentUser

Note : Install-Module downloads and installs the newest version of PowerShellGet into the current user's directory, $home\Documents\PowerShell\Modules.

Get-InstalledModule -Name Az -AllVersions

Get the Azure Subscription

Get-AzSubscription

Get all installed modules

Get-InstalledModule



Gets PowerShell repositories

Get-PSRepository

PowerShell Get

Get-Module -Name PowerShellGet


Get the AZ Tenant : Get the list of all the Tenants

Get-AzTenant

Get Context  : Explains about the current logged in Tenant

Get-AzContext

Get Context  : Explains about the Multiple Tenants

Get-AzContext -ListAvailable

Get-AzAccessToken

Get-AzAccessToken
Find a module by name

Find-Module -Name PowerShellGet

Find modules with similar names
Find-Module -Name PowerShell*
Find a module in a specific repository

Find-Module -Name PowerShellGet -Repository PSGallery




To check your PowerShell version

$PSVersionTable.PSVersion

Sign in to another Cloud

Command gets a list of available environments

Get-AzEnvironment | Select-Object -Property Name
Get-AzEnvironment

Command to Sign in to Different Environment
Connect-AzAccount -Environment AzureChinaCloud
