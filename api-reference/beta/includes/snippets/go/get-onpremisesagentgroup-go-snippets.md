---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2610850dc51bbc65cde783de996e2db44644f073
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092302"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.OnPremisesAgentGroupRequestBuilderGetQueryParameters{
    Expand: "publishedResources,agents",
}
options := &msgraphsdk.OnPremisesAgentGroupRequestBuilderGetOptions{
    Q: requestParameters,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
onPremisesAgentGroupId := "onPremisesAgentGroup-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).AgentGroupsById(&onPremisesAgentGroupId).Get(options)


```