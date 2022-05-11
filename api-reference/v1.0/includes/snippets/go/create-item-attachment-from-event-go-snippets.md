---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4df633260907eb2e8632432b7fdee59a92f4eb24
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322429"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttachment()
name := "Holiday event"
requestBody.SetName(&name)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.itemAttachment",
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Attachments().Post(requestBody)


```