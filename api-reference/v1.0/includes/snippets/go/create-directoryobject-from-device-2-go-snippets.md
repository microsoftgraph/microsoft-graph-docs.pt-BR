---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c96043ff1943c48ddabc5f89c13a6f115f10fd88
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323066"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
}
deviceId := "device-id"
directoryObjectId := "directoryObject-id"
graphClient.DevicesById(&deviceId).RegisteredUsersById(&directoryObjectId).Post(requestBody)


```