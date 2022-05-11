---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4d41e2d297b0f2183befaae5b19e2f58ddd4f46
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322851"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/users/{userId}",
}
printerShareId := "printerShare-id"
userId := "user-id"
graphClient.Print().SharesById(&printerShareId).AllowedUsersById(&userId).Post(requestBody)


```