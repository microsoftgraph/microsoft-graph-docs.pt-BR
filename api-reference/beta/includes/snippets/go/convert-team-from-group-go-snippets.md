---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4ac7ce5de142526d7e08c97e7718226fd0c645bd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001766"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTeam()
requestBody.SetChannels( []Channel {
    msgraphsdk.NewChannel(),
    SetAdditionalData(map[string]interface{}{
        "displayName": "Class Announcements 📢",
        "isFavoriteByDefault": true,
    }
    msgraphsdk.NewChannel(),
    SetAdditionalData(map[string]interface{}{
        "displayName": "Homework 🏋️",
        "isFavoriteByDefault": true,
    }
}
memberSettings := msgraphsdk.NewTeamMemberSettings()
requestBody.SetMemberSettings(memberSettings)
allowCreateUpdateChannels := false
memberSettings.SetAllowCreateUpdateChannels(&allowCreateUpdateChannels)
allowDeleteChannels := false
memberSettings.SetAllowDeleteChannels(&allowDeleteChannels)
allowAddRemoveApps := false
memberSettings.SetAllowAddRemoveApps(&allowAddRemoveApps)
allowCreateUpdateRemoveTabs := false
memberSettings.SetAllowCreateUpdateRemoveTabs(&allowCreateUpdateRemoveTabs)
allowCreateUpdateRemoveConnectors := false
memberSettings.SetAllowCreateUpdateRemoveConnectors(&allowCreateUpdateRemoveConnectors)
requestBody.SetInstalledApps( []TeamsAppInstallation {
    msgraphsdk.NewTeamsAppInstallation(),
    SetAdditionalData(map[string]interface{}{
        "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')",
    }
    msgraphsdk.NewTeamsAppInstallation(),
    SetAdditionalData(map[string]interface{}{
        "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "template@odata.bind": "https://graph.microsoft.com/beta/teamsTemplates('standard')",
    "group@odata.bind": "https://graph.microsoft.com/beta/groups('dbd8de4f-5d47-48da-87f1-594bed003375')",
}
options := &msgraphsdk.TeamsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Teams().Post(options)


```