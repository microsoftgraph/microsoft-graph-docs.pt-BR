---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1679900813e54f6ed05c368c13f5c36a67eb32d
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719105"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewReferenceUpdateSchema()
@odata.id := "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}"
requestBody.Set@odata.id(&@odata.id)
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).ConnectorGroup().$ref().Put(requestBody)


```