---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	definition = @(
		'{"HomeRealmDiscoveryPolicy":{"AccelerateToFederatedDomain":true,"PreferredDomain":"federated.example.edu","AlternateIdLogin":{"Enabled":true}}}'
	)
	displayName = "displayName-value"
	isOrganizationDefault = $true
}

New-MgPolicyHomeRealmDiscoveryPolicy -BodyParameter $params

```