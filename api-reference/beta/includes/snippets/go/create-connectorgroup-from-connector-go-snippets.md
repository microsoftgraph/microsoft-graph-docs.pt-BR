---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21919c5fd2ad488adc5f51f46f4a7497cc8e0a5a
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097595"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}",
}
options := &msgraphsdk.ConnectorGroupRequestBuilderPostOptions{
    Body: requestBody,
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
connectorId := "connector-id"
connectorGroupId := "connectorGroup-id"
graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).ConnectorsById(&connectorId).MemberOfById(&connectorGroupId).Post(options)


```