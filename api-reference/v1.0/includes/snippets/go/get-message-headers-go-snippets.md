---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef90c6bde843bf923cce1eb4c4ef2e87cbbbfab9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324481"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessageRequestBuilderGetQueryParameters{
    Select: "internetMessageHeaders",
}
options := &msgraphsdk.MessageRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```