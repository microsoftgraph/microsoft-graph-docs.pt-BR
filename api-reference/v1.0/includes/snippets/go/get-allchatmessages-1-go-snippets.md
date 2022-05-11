---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de4e19f63c89e3ad9fb6e0b57ac74ddad9b8a0bf
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322172"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.MessagesRequestBuilderGetQueryParameters{
    Top: 2,
}
options := &msgraphsdk.MessagesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Messages().GetWithRequestConfigurationAndResponseHandler(options, nil)


```