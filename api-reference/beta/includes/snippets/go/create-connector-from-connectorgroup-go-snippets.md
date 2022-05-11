---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8d90305803aa53a7e74f5ed1dd7d0d50ffbea3cb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324880"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}",
}
onPremisesPublishingProfileId := "onPremisesPublishingProfile-id"
connectorGroupId := "connectorGroup-id"
connectorId := "connector-id"
graphClient.OnPremisesPublishingProfilesById(&onPremisesPublishingProfileId).ConnectorGroupsById(&connectorGroupId).MembersById(&connectorId).Post(requestBody)


```