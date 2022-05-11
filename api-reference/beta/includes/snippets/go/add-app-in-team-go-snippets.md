---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 908cac8addaeda91e4f217e165139a497b0158de
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325226"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeamsAppInstallation()
requestBody.SetAdditionalData(map[string]interface{}{
    "teamsApp@odata.bind": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a",
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).InstalledApps().Post(requestBody)


```