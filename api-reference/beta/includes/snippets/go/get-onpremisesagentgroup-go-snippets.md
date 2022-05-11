---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33eca8f0fbb06f49ea1b1d2d1951ee8cfd163faa
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324922"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.OnPremisesAgentGroupRequestBuilderGetQueryParameters{
    Expand: "publishedResources,agents",
}
options := &msgraphsdk.OnPremisesAgentGroupRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
onPremisesAgentGroupId := "onPremisesAgentGroup-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).AgentGroupsById(&onPremisesAgentGroupId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```