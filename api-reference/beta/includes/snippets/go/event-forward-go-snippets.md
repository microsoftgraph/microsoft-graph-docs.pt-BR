---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e72513c3e49b841f519c41b9e5dee0bc93b9e3fc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322711"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetToRecipients( []Recipient {
    msgraphsdk.NewRecipient(),
    SetAdditionalData(map[string]interface{}{
    }
}
comment := "Dana, hope you can make this meeting."
requestBody.SetComment(&comment)
eventId := "event-id"
graphClient.Me().EventsById(&eventId).Forward(event-id).Post(requestBody)


```