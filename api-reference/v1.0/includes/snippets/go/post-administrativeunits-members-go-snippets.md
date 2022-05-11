---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4eab53c806a28af50fae62e8b2cbb222509e4055
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323411"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/groups/{id}",
}
administrativeUnitId := "administrativeUnit-id"
directoryObjectId := "directoryObject-id"
graphClient.Directory().AdministrativeUnitsById(&administrativeUnitId).MembersById(&directoryObjectId).Post(requestBody)


```