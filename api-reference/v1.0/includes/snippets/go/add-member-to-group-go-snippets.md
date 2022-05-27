---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13bfae8e4af7a10f12392191ec45bd2cb8e125eb
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694746"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/{id}",
}
groupId := "group-id"
result, err := graphClient.GroupsById(&groupId).Members().$ref().Post(requestBody)


```