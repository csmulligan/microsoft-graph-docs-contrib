---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
	subject = "Let's go for lunch"
	body = @{
		contentType = "HTML"
		content = "Does noon time work for you?"
	}
	start = @{
		dateTime = "2017-09-04T12:00:00"
		timeZone = "Pacific Standard Time"
	}
	end = @{
		dateTime = "2017-09-04T14:00:00"
		timeZone = "Pacific Standard Time"
	}
	recurrence = @{
		pattern = @{
			type = "weekly"
			interval = 1
			daysOfWeek = @(
				"Monday"
			)
		}
		range = @{
			type = "endDate"
			startDate = "2017-09-04"
			endDate = "2017-12-31"
		}
	}
	location = @{
		displayName = "Harry's Bar"
	}
	attendees = @(
		@{
			emailAddress = @{
				address = "AdeleV@contoso.com"
				name = "Adele Vance"
			}
			type = "required"
		}
	)
	allowNewTimeProposals = $true
}

# A UPN can also be used as -UserId.
New-MgUserEvent -UserId $userId -BodyParameter $params

```