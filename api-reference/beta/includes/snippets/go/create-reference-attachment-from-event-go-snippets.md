---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c615754f891e63afc9b37736926af0dd027d757
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322375"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAttachment()
name := "Personal pictures"
requestBody.SetName(&name)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.referenceAttachment",
    "sourceUrl": "https://contoso.com/personal/mario_contoso_net/Documents/Pics",
    "providerType": "oneDriveConsumer",
    "permission": "Edit",
    "isFolder": "True",
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).Attachments().Post(requestBody)


```