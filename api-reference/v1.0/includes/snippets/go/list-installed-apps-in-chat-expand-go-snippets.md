---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d83e7ca4e58839a7b6c7e83a4ed53c907b74d86
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325486"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.InstalledAppsRequestBuilderGetQueryParameters{
    Expand: "teamsAppDefinition($expand=bot)",
}
options := &msgraphsdk.InstalledAppsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).InstalledApps().GetWithRequestConfigurationAndResponseHandler(options, nil)


```