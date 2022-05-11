---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d217133b02d40c2c0b1090c3e5d2aa7ebe0ecd37
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323299"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTemporaryAccessPassAuthenticationMethod()
startDateTime, err := time.Parse(time.RFC3339, "2021-01-26T00:00:00.000Z")
requestBody.SetStartDateTime(&startDateTime)
lifetimeInMinutes := int32(60)
requestBody.SetLifetimeInMinutes(&lifetimeInMinutes)
isUsableOnce := false
requestBody.SetIsUsableOnce(&isUsableOnce)
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
}
userId := "user-id"
result, err := graphClient.UsersById(&userId).Authentication().TemporaryAccessPassMethods().Post(requestBody)


```