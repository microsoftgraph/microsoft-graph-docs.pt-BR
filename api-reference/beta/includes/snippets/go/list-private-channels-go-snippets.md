---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edfcda3913b2616b5a47b2e221f5d071b95201b9
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325060"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.ChannelsRequestBuilderGetQueryParameters{
    Filter: "membershipType%20eq%20'private'",
}
options := &msgraphsdk.ChannelsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Channels().GetWithRequestConfigurationAndResponseHandler(options, nil)


```