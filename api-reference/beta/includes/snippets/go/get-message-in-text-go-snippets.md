---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3acdf3857a4730ae781616519f2aeef9a1f03d81
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323695"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessageRequestBuilderGetQueryParameters{
    Select: "subject,body,bodyPreview,uniqueBody",
}
headers := map[string]string{
    "Prefer": "outlook.body-content-type="text""
}
options := &msgraphsdk.MessageRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
    Headers: headers,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```