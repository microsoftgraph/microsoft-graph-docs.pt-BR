---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbcb20ff82750c5465342d85ad6141def54b31a6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322707"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.EventRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview",
}
headers := map[string]string{
    "Prefer": "outlook.body-content-type="text""
}
options := &msgraphsdk.EventRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
eventId := "event-id"
result, err := graphClient.Me().EventsById(&eventId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```