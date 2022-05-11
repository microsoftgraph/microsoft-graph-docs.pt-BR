---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45f6cffdc105d506ff64a2eae98ffd246d6a8792
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322708"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EventRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview,organizer,attendees,start,end,location,locations",
}
options := &msgraphsdk.EventRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```