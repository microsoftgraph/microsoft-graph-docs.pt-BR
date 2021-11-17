---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 612e74236c1ba75f505c3b6705194514641108a6
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988445"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewTeamsAppInstallation()
requestBody.SetAdditionalData(map[string]interface{}{
    "teamsApp@odata.bind": "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a",
}
options := &msgraphsdk.InstalledAppsRequestBuilderPostOptions{
    Body: requestBody,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).InstalledApps().Post(options)


```