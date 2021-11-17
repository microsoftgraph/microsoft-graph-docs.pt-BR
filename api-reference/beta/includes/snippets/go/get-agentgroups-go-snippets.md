---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77a9cfadaae390dfdb69e576c8c9f00d148a0be9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028220"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.AgentGroupsRequestBuilderGetQueryParameters{
    Expand: "agents,publishedResources",
}
options := &msgraphsdk.AgentGroupsRequestBuilderGetOptions{
    Q: requestParameters,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).AgentGroups().Get(options)


```