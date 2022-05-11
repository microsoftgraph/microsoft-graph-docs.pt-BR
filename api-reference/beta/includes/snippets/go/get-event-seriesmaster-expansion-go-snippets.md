---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f14c94ea7ef36aef08f6702b664b2de62454efe
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322709"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EventRequestBuilderGetQueryParameters{
    Select: "subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences",
    Expand: "exceptionOccurrences",
}
options := &msgraphsdk.EventRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```