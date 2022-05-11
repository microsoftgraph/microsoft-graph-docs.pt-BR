---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4aa27b7dee95533e39838f7ef67bdd5d0552ca6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323742"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeamsAppInstallation()
requestBody.SetAdditionalData(map[string]interface{}{
    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a",
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).InstalledApps().Post(requestBody)


```