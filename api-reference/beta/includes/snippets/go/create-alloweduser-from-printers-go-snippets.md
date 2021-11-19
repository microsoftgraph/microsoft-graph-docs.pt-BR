---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4501dd9028818b5b2c7a42e3e24897786688481
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61104031"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/users/{id}",
}
options := &msgraphsdk.RefRequestBuilderPostOptions{
    Body: requestBody,
}
printerShareId := "printerShare-id"
result, err := graphClient.Print().SharesById(&printerShareId).AllowedUsers().$ref().Post(options)


```