---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c2e41e438fcccf4398488c1453165d7bf43adb1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322558"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/groups/{id}",
}
administrativeUnitId := "administrativeUnit-id"
directoryObjectId := "directoryObject-id"
graphClient.AdministrativeUnitsById(&administrativeUnitId).MembersById(&directoryObjectId).Post(requestBody)


```