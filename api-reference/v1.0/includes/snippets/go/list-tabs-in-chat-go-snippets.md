---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4476dfa06ba92f5eb65f27aa7239a37613109513
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323787"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.TabsRequestBuilderGetQueryParameters{
    Expand: "teamsApp",
}
options := &msgraphsdk.TabsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).Tabs().GetWithRequestConfigurationAndResponseHandler(options, nil)


```