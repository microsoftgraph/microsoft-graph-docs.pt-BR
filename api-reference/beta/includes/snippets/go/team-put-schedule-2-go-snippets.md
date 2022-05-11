---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c14d25ca7bd434e3348238395f77acb50fffc40f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322359"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "enabled": true,
    "timeZone": "America/Chicago",
    "provisionStatus": "Completed",
    "provisionStatusCode": nil,
    "openShiftsEnabled": true,
    "swapShiftsRequestsEnabled": true,
    "offerShiftRequestsEnabled": true,
    "timeOffRequestsEnabled": true,
    "timeClockEnabled": true,
}
teamId := "team-id"
graphClient.TeamsById(&teamId).Schedule().Put(requestBody)


```