---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Beta.Users

$params = @{
	accountEnabled = $true
	displayName = "Adele Vance"
	mailNickname = "AdeleV"
	userPrincipalName = "AdeleV@contoso.com"
	passwordProfile = @{
		forceChangePasswordNextSignIn = $false
		password = "xWwvJ]6NMw+bWH-d"
	}
}

New-MgBetaUser -BodyParameter $params

```