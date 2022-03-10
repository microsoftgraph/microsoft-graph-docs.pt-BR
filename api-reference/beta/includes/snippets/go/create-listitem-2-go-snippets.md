---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a393d36f433b064266fe2f009417c1a74ec24d22
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410894"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewFieldValueSet()
requestBody.SetAdditionalData(map[string]interface{}{
    "Color": "Fuchsia",
    "Quantity": ,
}
options := &msgraphsdk.FieldsRequestBuilderPatchOptions{
    Body: requestBody,
}
siteId := "site-id"
listId := "list-id"
listItemId := "listItem-id"
result, err := graphClient.SitesById(&siteId).ListsById(&listId).ItemsById(&listItemId).Fields().Patch(options)


```