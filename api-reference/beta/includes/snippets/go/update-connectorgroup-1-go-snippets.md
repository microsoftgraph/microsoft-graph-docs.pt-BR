---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 405a2c0d5a75a6713943d91cbc74b859e1b27ee9
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019953"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewConnectorGroup()
name := "Connector Group Demo"
requestBody.SetName(&name)
options := &msgraphsdk.ConnectorGroupsRequestBuilderPostOptions{
    Body: requestBody,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
result, err := graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).ConnectorGroups().Post(options)


```