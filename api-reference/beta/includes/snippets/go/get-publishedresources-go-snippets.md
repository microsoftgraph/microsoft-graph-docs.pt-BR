---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12ceb1bc8288814d8553c7ae6ddf01f891588212
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324579"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PublishedResourcesRequestBuilderGetQueryParameters{
    Expand: "agentGroups",
}
options := &msgraphsdk.PublishedResourcesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).PublishedResources().GetWithRequestConfigurationAndResponseHandler(options, nil)


```