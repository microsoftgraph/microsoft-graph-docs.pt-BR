---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f978bb306856cd2075d842a8c30cfad1a0de1b9f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093523"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "enabled": true,
    "timeZone": "America/Chicago",
}
options := &msgraphsdk.ScheduleRequestBuilderPutOptions{
    Body: requestBody,
}
teamId := "team-id"
graphClient.TeamsById(&teamId).Schedule().Put(options)


```