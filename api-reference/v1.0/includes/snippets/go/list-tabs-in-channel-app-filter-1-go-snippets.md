---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 654677af7e2442d81a63787ca1d3edb8080f56c0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325135"
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
teamId := "team-id"
channelId := "channel-id"
result, err := graphClient.TeamsById(&teamId).ChannelsById(&channelId).Tabs().GetWithRequestConfigurationAndResponseHandler(options, nil)


```