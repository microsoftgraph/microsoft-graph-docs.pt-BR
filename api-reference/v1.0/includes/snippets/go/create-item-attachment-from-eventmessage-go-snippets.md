---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53145d7a366cee66982932c3077b25ccad6aba89
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324759"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttachment()
name := "name-value"
requestBody.SetName(&name)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#Microsoft.OutlookServices.ItemAttachment",
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Attachments().Post(requestBody)


```