---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2d61a8bf824d5db0c78a074b3c69b8a78baf7b1
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322804"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/users/alexd@contoso.com",
}
groupId := "group-id"
directoryObjectId := "directoryObject-id"
graphClient.GroupsById(&groupId).RejectedSendersById(&directoryObjectId).Post(requestBody)


```