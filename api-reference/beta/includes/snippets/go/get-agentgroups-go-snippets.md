---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5d43244019ab0207923d6f6b037d582106ed572
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323881"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AgentGroupsRequestBuilderGetQueryParameters{
    Expand: "agents,publishedResources",
}
options := &msgraphsdk.AgentGroupsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).AgentGroups().GetWithRequestConfigurationAndResponseHandler(options, nil)


```