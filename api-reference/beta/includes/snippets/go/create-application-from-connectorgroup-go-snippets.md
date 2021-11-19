---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e589e3e8d806b89c58d41dfbb89192b320e652cd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097306"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}",
}
options := &msgraphsdk.RefRequestBuilderPutOptions{
    Body: requestBody,
}
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).ConnectorGroup().$ref().Put(options)


```