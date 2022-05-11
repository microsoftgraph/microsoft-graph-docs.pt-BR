---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 326e9a6d553ee0782b0dd7c126936593f055ec63
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322290"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.OnPremisesPublishingProfileRequestBuilderGetQueryParameters{
    Expand: "publishedResources,agents,agentGroups",
}
options := &msgraphsdk.OnPremisesPublishingProfileRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```