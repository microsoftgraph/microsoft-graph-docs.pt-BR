---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1b7f60782686ea0ee5653aa95aa1ce0aa333f24c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323085"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AllChannelsRequestBuilderGetQueryParameters{
    Filter: "membershipType%20eq%20'shared'",
}
options := &msgraphsdk.AllChannelsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).AllChannels().GetWithRequestConfigurationAndResponseHandler(options, nil)


```